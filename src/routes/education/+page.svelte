<script lang="ts">
	import LabeledList from '$lib/LabeledList.svelte';
	import School from '$lib/School.svelte';
</script>

<h1 class="page__title">Education</h1>

<School
	imageSource="northeastern.png"
	name="Northeastern University"
	location="Boston, MA"
	datesAttended="September 2021 – May 2025"
	subtitle="Khoury College of Computer Sciences"
	degree="Bachelor of Science, Computer Science and Physics"
/>

<LabeledList
	title="Honors and Awards"
	items={['Summa Cum Laude', 'Honors College', "Dean's List", 'Academic Excellence in Physics']}
/>
<hr />
<LabeledList
	title="Computer Science Courses"
	items={[
		'Software Engineering',
		'Artificial Intelligence',
		'Computer Systems',
		'Network Fundamentals',
		'Programming Languages',
		'Object-Oriented Design',
		'Theory of Computation',
		'Algorithms and Data',
		'Logic and Computation',
		'Fundamentals of Computer Science I and II'
	]}
/>
<hr />
<LabeledList
	title="Physics Courses"
	items={[
		'Electricity and Magnetism I and II',
		'Quantum Mechanics',
		'Thermodynamics and Statistical Mechanics',
		'Classical Dynamics',
		'Advanced Physics Laboratory',
		'Electronics',
		'Modern Physics',
		'Introductory Physics I and II'
	]}
/>
<hr />
<LabeledList
	title="Other Relevant Course&shy;work"
	items={[
		'Calculus I, II, and III',
		'Fourier Series and Partial Differential Equations',
		'Differential Equations and Linear Algebra',
		'Cryptography',
		'Probability and Statistics',
		'Advanced Technical Writing'
	]}
/>
