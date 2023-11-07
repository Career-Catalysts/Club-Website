<script lang="ts">
	import { T } from '@threlte/core'
	import { Align, Float, OrbitControls } from '@threlte/extras'

	const count = 250
	const positions = new Float32Array(count * 3)

	for (let i = 0; i < count; i++) {
		positions[i * 3] = (Math.random() - 0.5) * 3
		positions[i * 3 + 1] = (Math.random() - 0.5) * 5.5
		positions[i * 3 + 2] = -10 - Math.random() * 1
	}

	const sizes = {
		width: window.innerWidth,
		height: window.innerHeight,
	}

	const cursor = {
		x: 0,
		y: 0,
	}

	window.addEventListener('mousemove', (event) => {
		cursor.x = event.clientX / sizes.width - 0.5
		cursor.y = event.clientY / sizes.height - 0.5
	})

	let scrollY = window.scrollY

	window.addEventListener('scroll', () => {
		scrollY = window.scrollY
	})
</script>

<T.Group position={[cursor.x * 0.1, cursor.y * 0.1, 0]}>
  <T.PerspectiveCamera makeDefault position={[0, -scrollY / sizes.height, 6]} fov={35}>
    <OrbitControls />
  </T.PerspectiveCamera>
</T.Group>

<Float floatingRange={[-0.03, 0.03]}>
<Align>
	<T.Points>
		<T.BufferGeometry>
			<T.BufferAttribute
				args={[positions, 3]}
				attach={(parent, self) => {
					parent.setAttribute('position', self)
				}}
			/>
		</T.BufferGeometry>
		<T.PointsMaterial sizeAttenuation={true} size={0.03} />
	</T.Points>
</Align>
</Float>
