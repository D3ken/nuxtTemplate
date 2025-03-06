<script setup>

</script>

<template>
	<div class="wrap">
		<nav class="navigation">
			<div class="container">
				<div class="navigation__inner">
					<ul class="navigation__inner-widgets-list">
						<li class="navigation__inner-widgets-list-item">
							<a href="#">
								<img src="../public/image/location.svg" alt="#" />
								<span>Москва</span>
							</a>
						</li>
						<li class="navigation__inner-widgets-list-item">
							<a href="#">
								<img src="../public/image/delivery.svg" alt="#" />
								<span>Доставка и оплата</span>
							</a>
						</li>
						<li class="navigation__inner-widgets-list-item">
							<a href="#">
								<img src="../public/image/adress.svg" alt="#" />
								<span>Адрес и часы работы</span>
							</a>
						</li>
					</ul>
					<ul class="navigation__inner-contacts">
						<li class="navigation__inner-contacts-list">
							<a href="#"><img src="../public/image/mail.svg" alt="#" />
								<span>market@estatut.ru</span>
							</a>
						</li>
						<li class="navigation__inner-contacts-list">
							<a href="#">
								<img src="../public/image/phone.svg" alt="#" />
								<span>8 (968) 660-65-50</span>
								<img src="../public/image/info.svg" alt="#" />
							</a>
						</li>
					</ul>
				</div>
			</div>
		</nav>
		<header class="header">
			<div class="container">
				<div class="header__inner">
					<div class="header__inner-search">
						<a href="#">
							<img src="../public/image/logoMain.png" alt="#" />
						</a>
						<div class="search-block">
							<input
								placeholder=" Автор, название, ISBN"
								type="text"
								name=""
								id=""
							/>
							<button>
								<img src="../public/image/searchIcon.svg" alt="#" />
								<span>Искать</span>
							</button>
						</div>
					</div>
					<div class="header__inner-auth">
						<ul class="header__inner-auth-list">
							<li class="header__inner-auth-list-item">
								<a href="#">
									<img src="../public/image/laterIcon.svg" alt="#" />
									<span>Отложено</span>
								</a>
							</li>
							<li class="header__inner-auth-list-item">
								<a href="#">
									<img src="../public/image/loginIcon.svg" alt="#" />
									<span>Войти</span>
								</a>
							</li>
							<li class="header__inner-auth-list-item">
								<a href="#">
									<img src="../public/image/cartIcon.svg" alt="#" />
									<span>Корзина</span>
								</a>
							</li>
						</ul>
					</div>
				</div>
			</div>
		</header>
		<section class="catalog">
			<div class="container">
				<div class="catalog__inner">
					<ul class="catalog__inner-list">
						<li class="catalog__inner-list-item">
							<a href="#">
								<img src="../public/image/catalogIcon.svg" alt="#"/>
								<span>Каталог</span>
							</a>
						</li>
						<li class="catalog__inner-list-item">
							<a href="#"><span>Авторы</span></a>
						</li>
						<li class="catalog__inner-list-item">
							<a href="#"><span>Новинки</span></a>
						</li>
						<li class="catalog__inner-list-item">
							<a href="#">
								<img src="../public/image/actionsicon.svg" alt="#" />
								<span class="sale">Скидки</span>
							</a>
						</li>
						<li class="catalog__inner-list-item">
							<a href="#"><span>Партнерам</span></a>
						</li>
						<li class="catalog__inner-list-item">
							<a href="#"><span>Мы</span></a>
						</li>
					</ul>
				</div>
			</div>
		</section>
	</div>
	<div class="media-header">
		<div class="container">
			<ul class="media-header-list">
				<li class="media-header-list-item first">
					<img src="../public/image/catalogIcon.svg" alt="#"/>
				</li>
				<li class="media-header-list-item second">
					<img src="../public/image/logoMain.png" alt="#" />
				</li>
				<li class="media-header-list-item media-search">
					<input placeholder="Что будем искать?" type="text" />
					<button>
						<img src="../public/image/searchIconMini.svg" alt="#" />
					</button>
				</li>
				<li class="media-header-list-item last">
					<img src="../public/image/cartIcon.svg" alt="#" />
				</li>
			</ul>
		</div>
	</div>
</template>

<style>
* {
	box-sizing: border-box;
	color: var(--text-main-color);
	font-size: var(--text-main-size);
}

a {
	text-decoration: none;
}

p {
	margin: 0;
	margin-bottom: 8px;
}
img {
	border-radius: 5px;
}
li {
	list-style-type: none;
}
ul {
	padding: 0px;
	margin: 0px;
}
body {
	font-family: 'Roboto', serif;
	background-color: rgba(249, 249, 250, 1);
}

:root {
	--text-main-color: #1c294dcc;
	--text-main-size: 14px;
	--text-sale-red-bright: #fd3a3a;
	--text-sale-red-muted: #ff283d;
	--text-huge-weight: 700;
	--text-big-weight: 500;
	--text-big-size: 16px;
}
.wrap {
	background-color: #fff;
	padding: 0px 116px;
}
.container {
	width: 100%;
	max-width: 1140px;
	margin: 0 auto;
	padding: 0px;
}
.navigation {
	margin-bottom: 20px;
	border-bottom: 1px solid gray;
}

.navigation__inner {
	display: flex;
	justify-content: space-between;
	align-items: center;
}

.navigation__inner ul {
	display: flex;
	padding: 17px 0px;
	gap: 37px;
}

.navigation__inner ul li a {
	display: flex;
	align-items: center;
	gap: 5px;
}

.navigation__inner-widgets-list {
	padding: 0px;
}
.navigation__inner-contacts li {
	color: var(--text-big-size);
	font-weight: var(--text-big-weight);
}

.header__inner {
	display: flex;
	justify-content: space-between;
	align-items: center;
	margin-bottom: 24px;
}

.header__inner-search {
	display: flex;
	align-items: center;
	gap: 30px;
}

.search-block {
	display: flex;
}

.search-block input {
	padding: 10px;
	width: 450px;
	border: 1px solid #dfe0e1;
	border-right: none;
	border-radius: 5px 0px 0px 5px;
}

.search-block button {
	display: flex;
	align-items: center;
	background-color: #ff7a00;
	border: 1px solid #ff7a00;
	border-left: none;
	gap: 5px;
	width: 123px;
	border-radius: 0px 5px 5px 0px;
}

.search-block button img {
	margin-left: 26px;
}

.search-block button span {
	color: #fff;
}

.header__inner-auth-list {
	display: flex;
	gap: 35px;
}

.header__inner-auth-list-item a {
	display: flex;
	gap: 5px;
	align-items: center;
}

.catalog__inner-list {
	display: flex;
	padding-top: -1px;
	gap: 25px;
}

.catalog__inner-list-item a {
	display: flex;
	align-items: start;
	gap: 5px;
}

.sale {
	color: var(--text-sale-red-muted);
}

.media-header {
	display: none;
	margin-bottom: 10px;
}

@media (max-width: 890px) {
	.media-header {
		display: block;
		height: 70px;
		margin-bottom: 0;
	}
	.navigation {
		display: none;
	}
	.header {
		display: none;
	}
	.catalog {
		display: none;
	}
	.container {
		max-width: 375px;
		display: flex;
		align-items: center;
		height: 100%;
		padding: 0px;
		justify-content: center;
	}
	.media-header-list {
		display: flex;
		align-items: center;
		justify-content: space-evenly;
		height: 100%;
		width: 100%;
	}
	.media-search {
		display: flex;
	}
	.media-search input {
		padding: 2px 0 2px 10px;
		height: 40px;
		border-radius: 5px 0px 0px 5px;
		border: none;
		border-right: none;
		background-color: #f7f7f7;
		max-width: 170px;
	}
	.media-search button {
		border: none;
		background-color: #f7f7f7;
		padding: 10px 12px;
		border-radius: 0px 5px 5px 0px;
	}
	.second img{
		width: 44px;
		height: 35px;
	}
}
</style>
