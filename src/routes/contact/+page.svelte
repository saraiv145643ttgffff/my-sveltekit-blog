<script>
	import { createBubbler, preventDefault } from 'svelte/legacy';

	const bubble = createBubbler();
	import Callout from '$lib/components/Callout.svelte'
</script>


<svelte:head>
	<title>Contact</title>
</svelte:head>


<h1>Góp ý</h1>

Bạn có thể  <a rel="external" href="https://docs.google.com/forms/d/e/1FAIpQLSeRCq0W8eQDnwnt4dS5crKctEPcsV_nXrD0rRo3kc6Veyn4uQ/viewform?usp=header">ấn vào đây</a> nếu có bất kì góp nào.

<form onsubmit={preventDefault(bubble('submit'))}>
	<div class="form-section">
		<label for="name">Họ và Tên</label>
		<input type="text" id="name" placeholder="Họ và Tên" />
	</div>
	
	<div class="form-section">
		<label for="email">Email</label>
		<input type="email" id="email" placeholder="Địa chỉ email " />
	</div>

	<fieldset>
		<legend>
			Giới tính 
		</legend>

		<div>
			<input type="radio" name="s" id="s1" value="s1">
			<label for="s1">Nam </label>
		</div>
		<div>
			<input type="radio" name="s" id="s2" value="s2">
			<label for="s2">Nữ </label>
		</div>
	</fieldset>

	<div class="form-section">
		<input type="checkbox" id="c1" >
		<label for="c1">Tích nếu bạn hài lòng!</label>
	</div>

	<input type="submit" value="Lưu">
</form>