<script setup>

</script>

<template>
	<section class="socials">
		<div class="container">
			<ul class="socials__inner-media-links">
				<li>
					<a href=""><img src="../public/image/FacebookMini.svg" alt="#" /></a>
				</li>
				<li>
					<a href=""><img src="../public/image/VkMini.svg" alt="#" /></a>
				</li>
				<li>
					<a href=""><img src="../public/image/InstagramMini.svg" alt="#" /></a>
				</li>
			</ul>
			<div class="socials__inner">
				<img src="../public/image/logoMain.png" alt="#" />
				<div class="socials__inner-search-block search-block">
					<input
						placeholder="Введите свой Email и получите скидку"
						type="text"
					/>
					<button><img src="../public/image/fly.svg" alt="#" /></button>
				</div>

				<ul class="socials__inner-links">
					<li>
						<a href=""><img src="../public/image/FacebookIcon.svg" alt="#" /></a>
					</li>
					<li>
						<a href=""><img src="../public/image/InstagramIcon.svg" alt="#" /></a>
					</li>
					<li>
						<a href=""><img src="../public/image/TwitterIcon.svg" alt="#" /></a>
					</li>
				</ul>
			</div>
		</div>
	</section>
</template>

<style>

.socials {
	padding-bottom: 20px;
    padding-top: 20px;
    background-color: #F9F9FA;
}

.socials__inner {
    background-color: #F9F9FA;
	display: flex;
	align-items: center;
	justify-content: space-between;
}

.socials__inner .search-block > input {
	width: 393px;
}

.socials__inner .search-block > button {
	width: 50px;
	justify-content: center;
}

.socials__inner .search-block > button img {
	margin-left: 0px;
}

.socials__inner-links {
	display: flex;
	gap: 15px;
}

.socials__inner-media-links {
	display: none;
}

@media (max-width: 890px) {
    .socials > .container{
        flex-direction: column;
    }
	.socials__inner-links {
		display: none;
	}

	.socials__inner {
		justify-content: unset;
		gap: 15px;
		padding-bottom: 20px;
	}

	.socials__inner .search-block > input {
		width: 220px;
	}

	.socials__inner .search-block {
		margin-left: auto;
	}
	.socials__inner-media-links {
		display: flex;
		gap: 15px;
		align-items: center;
		justify-content: center;
		padding-bottom: 20px;
		border-bottom: 1px solid rgba(28, 41, 77, 0.15);
		margin-bottom: 20px;
        width: 100%;
	}
}
</style>
