<script setup>

</script>

<template>
	<section class="promos">
		<div class="container">
			<div class="promos__inner">
				<div class="promos__inner-grid-container">
					<div class="promos__inner-slider">
						<img src="../public/image/sliderIMG.svg" alt="#" />
						<img 
                            class="promos__daily-picture-arrow-left absolute"
							src="../public/image/Arrow.svg"
							alt="#"
						/>
						<img
							class="promos__daily-picture-arrow-right absolute"
							src="../public/image/Arrow.svg"
							alt="#"
						/>
					</div>
					<div class="promos__inner-daily">
						<div class="promos__daily-heading">
							<h3>Книга дня</h3>
							<span>08:56:31</span>
						</div>
						<div class="promos__daily-picture">
							<img class="slider" src="../public/image/bookGirlImage.png" alt="#" />
						</div>
						<div class="promos__daily-caption">
							<p class="promos__daily-caption-genre">Корпоративное право</p>
							<p class="promos__daily-caption-name">
								Инвестирование: способы, риски, субъекты : монография
							</p>
							<p class="promos__daily-caption-author">Майфат А.В.</p>
							<p class="promos__daily-caption-price">4 450 ₽</p>
						</div>
						<div class="promos__daily-btns template-btns">
							<button>
								<img src="../public/image/orangeCart.svg" alt="#" />
								<span>В корзину</span>
							</button>
							<button>
								<img src="../public/image/laterIcon.svg" alt="#" />
							</button>
						</div>
					</div>
					<div class="promos__inner-offers">
						<div class="promos__inner-offers-shipping">
							<p>Бесплатно доставим ваш заказ при покупке от 2000 ₽</p>
							<img
								class="promos__inner-offers-shipping-accessory absolute"
								src="../public/image/vectorLine.svg"
								alt="#"
							/>
							<img src="../public/image/manImg.png" alt="#" />
						</div>
						<div class="promos__inner-offers-register-sale">
							<p>
								Скидка <br />
								при регистрации<br />
								до 15%
							</p>
							<img
								class="promos__inner-offers-register-sale-accessory absolute"
								src="../public/image/vector2.png"
								alt="#"
							/>
							<img src="../public/image/mainImg2.png" alt="#" />
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<style>

.promos {
	padding-top: 30px;
    margin-top: 20px;
    background-color: #F9F9FA;
}

.promos__inner {
	padding-bottom: 30px;
}
.promos__inner-slider {
	grid-area: slider;
}

.promos__inner-daily {
	grid-area: daily;
	background-color: #FFFFFF;
	border-radius: 5px;
    display: flex;
	max-width: 360px;
	flex-direction: column;
	padding: 20px 20px 20px 20px;
}

.promos__inner-offers {
	grid-area: offers;
}

.promos__inner-grid-container {
	display: grid;
    grid-template-columns: 360px 360px 360px;
    grid-template-rows: auto auto;
	grid-template-areas:
		'slider slider daily'
		'slider slider daily'
		'offers offers daily';
	grid-gap: 20px;
}
.promos__daily-picture {
	align-self: center;
	margin-bottom: 15px;
}
.promos__daily-heading {
	display: flex;
	align-items: center;
	justify-content: space-between;
	margin-bottom: 20px;
}

.promos__daily-heading h3 {
	font-size: 16px;
	font-weight: 500;
}

.promos__daily-heading span {
	padding: 5px 10px;
	color: #ff7a00;
	background-color: rgba(255, 122, 0, 0.15);
	border-radius: 5px;
}

.promos__daily-caption p:first-child {
	font-size: 12px;
	color: rgba(28, 41, 77, 0.5);
	margin-bottom: 8px;
}

.promos__daily-caption p:nth-child(2) {
	color: rgba(28, 41, 77, 1);
	font-weight: 500;
	margin-bottom: 8px;
	font-size: 12px;
}

.promos__daily-caption p:last-child {
	color: rgba(28, 41, 77, 1);
	font-size: 18px;
	font-weight: 700;
	margin-bottom: 12px;
}

.template-btns {
	display: flex;
	align-items: center;
	gap: 10px;
}

.template-btns button {
	border: 1px solid rgba(238, 238, 238, 1);
	border-radius: 5px;
	background-color: #fff;
}

.template-btns button:first-child {
	display: flex;
	align-items: center;
	padding: 12px 25px;
	gap: 12px;
}
.template-btns button span {
	color: rgba(28, 41, 77, 1);
	font-weight: 600;
}
.template-btns button:last-child {
	padding: 12px 15px;
}

.absolute {
	position: absolute;
}

.promos__inner-slider {
	position: relative;
}

.promos__daily-picture-arrow-left {
	left: 0;
	top: 32%;
    cursor: pointer;
}

.promos__daily-picture-arrow-right {
	right: 0;
	top: 32%;
    cursor: pointer;
    transform: rotate(180deg);
}

.promos__inner-offers {
	display: flex;
	align-items: center;
	gap: 30px;
}

.promos__inner-offers-shipping {
	display: flex;
	background-color: rgba(109, 55, 143, 1);
    width: 360px;
    height: 140px;
	border-radius: 5px;
	gap: 13px;
    display: flex;
    justify-content: center;
    align-items: center;
	position: relative;
}

.promos__inner-offers-shipping p {
	max-width: 199px;
	color: rgba(255, 255, 255, 1);
	z-index: 100;
	font-size: 20px;
}

.promos__inner-offers-shipping-accessory {
	z-index: 1;
	top: 15%;
	left: 3%;
}

.promos__inner-offers-register-sale {
	display: flex;
}

.promos__inner-offers-register-sale {
	display: flex;
	background-color: rgba(255, 216, 239, 1);
	width: 360px;
    height: 140px;
    max-height: 140px;
	border-radius: 5px;
	position: relative; 
    justify-content: center;
    align-items: center;
}

.promos__inner-offers-register-sale p {
	max-width: 199px;
	color: rgba(28, 41, 77, 0.8);
	z-index: 100;
	font-size: 20px;
    
}

.promos__inner-offers-register-sale-accessory {
	bottom: 30px;
	left: 14%;
}

.promos__inner-offers-register-sale {
	height: 165px;
}

@media (max-width: 890px) {
	.promos__inner .promos__inner-grid-container {
		display: grid;
		grid-template-areas:
			'slider slider slider'
			'daily daily daily '
			'offers offers offers';
		grid-gap: 30px;
		grid-template-columns: auto auto auto;
	}

	.promos__inner-offers-shipping-accessory {
		top: 16%;
	}

	.promos__inner .promos__inner-slider img:first-child {
		width: 355px;
		height: 175px;
	}
	.promos__daily-picture-arrow-left absolute {
		display: none;
	}
	.promos__inner .promos__daily-picture-arrow-right img {
		display: none;
	}
	.promos__inner {
		padding: 5px;
	}
	.promos__inner-offers {
		flex-direction: column;
	}

	.promos__inner-offers-shipping p {
		font-size: 19px;
	}

	.promos__daily-picture-arrow-right {
		display: none;
	}

	.promos__daily-picture-arrow-left {
		display: none;
	}

	.promos {
		padding-top: 0px;
	}

	.promos__inner .promos__inner-grid-container {
		grid-gap: 10px;
	}

	.promos__inner-offers {
		gap: 10px;
	}

	.promos {
		padding-bottom: 10px;
		margin-bottom: 0px;
	}
}
</style>
