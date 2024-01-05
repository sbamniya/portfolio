<script>
	import Button from '../button/index.svelte';
	import DownloadImage from './../../assets/images/icons/download.png';
</script>

<a href="/Sonu_FullStack_8Years.pdf" download="Sonu_FullStack_8Years.pdf">
	<Button variant="icon">
		Download CV
		<img src={DownloadImage} alt="DownloadImage" />
	</Button>
</a>
