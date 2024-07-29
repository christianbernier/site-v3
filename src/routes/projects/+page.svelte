<script lang="ts">
	import Project from '$lib/Project.svelte';
</script>

<h1 class="page__title">Projects</h1>

<Project
	title="Fourier Fun"
	dates="June 2024"
	link="https://fourier.cbernier.com"
	technologies="TypeScript, C++ (WASM), SvelteKit"
	bullets={[
		'Created interactive demonstration of using the Discrete Fourier Transform to approximate a 2D path',
		'Explored WebAssembly to enhance the speed of calculations for user-generated paths'
	]}
/>

<Project
	title="Photo Blog"
	dates="December 2023 – February 2024"
	link="https://blog.cbernier.com"
	technologies="TypeScript, SvelteKit, PostgreSQL"
	bullets={[
		'Developed personal blog to post a photo every day, served by a PostgreSQL database and S3 bucket',
		'Implemented automatic image compression for the ability to quickly add photos on-the-go'
	]}
/>

<Project
	title="Solenoid Magnetic Field Visualization"
	dates="December 2023"
	technologies="Python"
	bullets={[
		'Visualized the magnetic field of a customizable non-infinite solenoid through an interactive 3D environment',
		'Learned about numerical integration, 3D plotting, and matrix operations in NumPy'
	]}
/>

<Project
	title="Six-Letter Wordle"
	dates="August 2023"
	link="https://wordle.cbernier.com"
	technologies="TypeScript, React"
	bullets={[
		"Created version of the New York Times's popular word game Wordle using 6 letters instead of 5",
		'Learned about multi-component state management using custom Redux-like implementation'
	]}
/>

<Project
	title="Spotify Roulette"
	dates="December 2022 – February 2023"
	link="https://spotify.cbernier.com"
	technologies="JavaScript, React, NodeJS"
	bullets={['Developed song-guessing game using the Spotify API']}
/>

<Project
	title="Graphical Image Processing and Enhancement Application"
	dates="June 2022"
	technologies="Java"
	bullets={[
		'Developed GUI application to manipulate and analyze image files using Java Swing for Object-Oriented Design class',
		'Utilized model-view-controller design with kernel filtering and linear color transformation classes for easy editing',
		'Explored object-oriented principles such as the Builder, Command, Adapter, Decorator, and Strategy design patterns'
	]}
/>

<Project
	title="Physics Notes Generator"
	dates="January 2022 – April 2022"
	link="https://physics.notes.cbernier.com"
	technologies="JavaScript, NodeJS"
	bullets={[
		'Created a static site generator to parse my physics notes from Markdown/LaTeX into HTML using 	NodeJS',
		'Boosted productivity of study sessions significantly by making notes easy to access and well-	organized'
	]}
/>

<Project
	title="Special Relativity"
	dates="January 2022"
	link="https://relativity.cbernier.com"
	technologies="JavaScript, React"
	bullets={[
		'Made an interactive spacetime diagram to visualize Lorentz transformations used in special relativity',
		'Implemented various equations used in modern physics to provide an intuition behind the math of relativity'
	]}
/>

<Project
	title="Gerrymander Me!"
	dates="July 2020 – October 2020"
	link="https://gerrymanderme.cbernier.com"
	technologies="JavaScript, React"
	bullets={[
		'Built a game in JavaScript, HTML, and CSS to demonstrate the effects of partisan gerrymandering',
		'Delivered an engaging and interactive experience to over 100 students in AP U.S. Government classes'
	]}
/>

<Project
	title="Lissajous Curves"
	dates="February 2021"
	link="https://lissajous.cbernier.com"
	technologies="JavaScript, React"
	bullets={[
		'Developed an interactive tool to visualize complex harmonic motion found in physical systems',
		'Provides users the ability to change parameters of the systems and observe how the resulting patterns are affected'
	]}
/>

<Project
	title="MBTA Wiki"
	dates="March 2018 – August 2020"
	link="https://mbta.cbernier.com"
	technologies="JavaScript, React, React Native"
	bullets={[
		'Created a reference website and iOS app to track trains and buses on Boston public transit network',
		'Generated over 1,000 iOS app downloads and thousands of website pageviews with reliable and useful information',
		'Learned HTML, JavaScript, CSS, and React to present third-party API data in a fast and organized way'
	]}
/>

<Project
	title="3D Fractal Visualizer"
	dates="April 2019 – June 2019"
	technologies="Java, C/C++"
	bullets={[
		'Developed an interactive program to visualize complex 3D fractals using for AP Computer Science class with a partner',
		'Utilized distance estimator and ray-marching rendering methods in Java/C program with LWJGL library for graphics'
	]}
/>
