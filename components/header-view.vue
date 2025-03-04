<script setup>

</script>

<template>
	<div class="container">
		<div class="container-inner">
			<div class="header-line__top-block">
				<div class="top-block__delivery">
					<div class="delivery__location del_box">
						<a class="delivery-box__links" href="#">
							<img src="../public/image/location.svg" alt="#">
							Москва
						</a>
					</div>
					<div class="delivery__box del_box">
						<a class="delivery-box__links" href="#">
							<img src="../public/image/delivery.svg" alt="#">
							Доставка и оплата
						</a>
					</div>
					<div class="delivery__address del_box">
						<a class="delivery-box__links" href="#">
							<img src="../public/image/adress.svg" alt="#">
							Адрес и часы работы
						</a>
					</div>
				</div>
				<div class="top-block__contacts">
					<div class="contacts__mail">
						<a href="#" class="contacts-box__links">
							<img src="../public/image/mail.svg" alt="#">
							market@estatut.ru
						</a>
					</div>
					<div class="contacts__number">
						<a href="#" class="contacts-box__links">
							<img src="../public/image/phone.svg" alt="#">
							8 (968) 660-65-50
							<img class="info-icon" src="../public/image/info.svg" alt="#">
						</a>
					</div>
				</div>
			</div>
			<div class="header-line__bottom-block" >
				<div class="bottom-block__top-side" id="top">
					<div class="bottom-block__search-box">
						<img src="../public/image/logoMain.png" alt="#">
						<div class="search-box">
							<input class="search-box__input" type="text" placeholder="Автор, название, ISBN">
							<button class="search-box__button">
								<img src="../public/image/searchIcon.svg" alt="#">
								Искать
							</button>
						</div>
					</div>
					<div class="bottom-block__menu-box">
						<div class="menu-box__button">
							<img class="menu-box_img" src="../public/image/laterIcon.svg" alt="#">
							Отложено
						</div>
						<div class="menu-box__button">
							<img class="menu-box_img" src="../public/image/loginIcon.svg" alt="#">
							Войти
						</div>
						<div class="menu-box__button">
							<div class="score-box">
								<span class="score-box__number">10</span>
								<img class="menu-box_img" src="../public/image/cartIcon.svg" alt="#">
							</div>
							Корзина
						</div>
					</div>
				</div>
				<div class="bottom-block__bottom-side" id="bottom">
					<nav class="header__navigate">
						<ul class="navigate__list">
							<li class="list__link catalog-link">
								<a href="#">
									<img src="../public/image/catalogIcon.svg" alt="#">
									Каталог
								</a>
							</li>
							<li class="list__link">
								<a href="#">
									Авторы
								</a>
							</li>
							<li class="list__link">
								<a href="#">
									Новинки
								</a>
							</li>
							<li class="list__link fees-link">
								<a href="#">
									<img src="../public/image/actionsicon.svg" alt="#">
									Скидки
								</a>
							</li>
							<li class="list__link">
								<a href="#">
									Партнёрам
								</a>
							</li>
							<li class="list__link">
								<a href="#">
									Мы
								</a>
							</li>
						</ul>
					</nav>
				</div>
			</div>	
		</div>
	</div>
</template>

<style lang="scss">
	a{
		display: flex;
		font-family: Roboto;
		font-size: 14px;
		color: #1C294DCC;
	}
	button{
		font-family: Roboto;
	}
    .container{
		padding: 0px;
		display: flex;
		align-items: center;
		justify-content: center;
		margin: 0 auto;
		width: 1366px;
	}
	.container-inner{
		width: calc(100% - 226px);
	}
	.header-line__top-block{
		width: 100%;
		height: 51px;
		display: flex;
		justify-content: space-between;
		align-items: center;
	}
	.top-block__delivery{
		width: 50%;
		display: flex;
		align-items: center;
	}
	.del_box{
		display: flex;
		margin-right: 31px;
	}
	.top-block__contacts{
		width: 50%;
		display: flex;
		align-items: center;
		justify-content: flex-end;
	}
	.delivery-box__links img{
		margin-right: 5px;
	}
	.contacts-box__links{
		font-weight: 500;
		margin-left: 33px;
	}
	.contacts-box__links img:first-child{
		margin-right: 6px;
	}
	.info-icon{
		margin-left: 6px;
	}
	.header-line__bottom-block{
		width: 100%;
		height: 120px;
		border-top: 1px solid #DFE0E1;
	}
	.bottom-block__top-side{
		width: 100%;
		height: 40px;
		margin-top: 20px;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.bottom-block__bottom-side{
		width: 100%;
		display: flex;
		align-items: center;
		margin-top: 20px;
	}
	.bottom-block__search-box{
		display: flex;
		align-items: center;
		height: 100%;
	}
	.search-box{
		height: 100%;
		display: flex;
		align-items: center;
		border-radius: 5px;
		margin-left: 30px;
	}
	.search-box__input{
		width: 450px;
		height: 100%;
		display: flex;
		align-items: center;
		padding: 10px 0 14px 15px;
		border: 1px solid #DFE0E1;
		border-radius: 5px 0 0 5px;
		border-right: none;
		outline: none;
	}
	.search-box__input::placeholder{
		font-size: 14px;
		font-family: Roboto;
	}
	.search-box__button{
		height: 100%;
		justify-content: center;
		color: white;
		display: flex;
		align-items: center;
		width: 123px;
		border: none;
		background-color: #FF7A00;
		border-radius: 0 5px 5px 0;
		font-size: 14px;
	}
	.search-box__button img{
		margin-right: 6.67px;
	}
	.bottom-block__menu-box{
		display: flex;
	}
	.bottom-block__menu-box > div{
		display: flex;
		align-items: center;
		font-family: Roboto;
		font-size: 14px;
		margin-left: 30px;
	}
	.menu-box__button{
		cursor: pointer;
	}
	.menu-box_img{
		margin-right: 5px;
	}
	.score-box{
		position: relative;
	}
	.score-box__number{
		position: absolute;
		display: block;
		display: flex;
		align-items: center;
		justify-content: center;
		width: 15px;
		height: 15px;
		border-radius: 50%;
		background-color: #FF7A00;
		font-size: 9px;
		color: white;
		right: -2px;
		top: -7px;
	}
	.navigate__list{
		display: flex;
		align-items: center;
	}
	.list__link{
		margin-right: 25.5px;
		display: flex;
		align-items: center;
	}
	.list__link a{
		font-size: 14px;
	}
	.catalog-link > a > img{
		margin-right: 5px;
	}
	.fees-link > a > img{
		margin-right: 5px;
	}
	.fees-link > a{
		color: #FF283D;
	}

	@media (max-width: 376px) {
		.container{
			width: 100%;
			margin: 0px;
		}
		.container-inner{
			width: 100%;
		}
		.header-line__top-block{
			display: none;
		}
		.search-box__input{
			width: 195px;
		}
		.header-line__bottom-block{
			display: flex;
		}
		#top{
			order: 2;
		}
		#bottom{
			order: 1;
		}
		.header__navigate{
			display: none;
		}
		.catalog-link > img{
			display: block ;
		}
	}
</style>
