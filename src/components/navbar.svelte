
<script>
    import logo from "../assets/logo.static.svg";
</script>

<nav class="sticky top-0 m-0 z-10 ">
	<div class="flex justify-between items-center max-w-6xl mx-auto py-1 border-b bg-color">
		<a class="text-black text-lg " href="/">
			<img class="w-20" src={logo} alt="logo" />
		</a>

		<ul class=" hidden md:flex text-gray-500  align-middle items-center font-light ">
			<li>
				<a class=" hover:text-gray-900 special" href="#">Tadm</a>
			</li>
			<li>
				<p  class=" text-gray-400" href="#faq">Faq</p>
			</li>
			<li>
				<p class=" text-gray-400" href="#home">About</p>
			</li>

			<li>
				<p class=" text-gray-400" href="#home">Blog</p>
			</li>
		</ul>

		<a href="/" class="uppercase flex justify-center items-center gap-1 text-blue-800"
			>Preorder Now <svg width="7" height="10" xmlns="http://www.w3.org/2000/svg">
				<path
					d="M1.566.434 6.131 5 1.566 9.566.434 8.434 3.869 5 .434 1.566z"
					fill="currentColor"
				/>
			</svg></a
		>
	</div>
</nav>
