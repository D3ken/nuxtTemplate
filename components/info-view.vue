<script setup>

</script>

<template>
	<section class="credits">
		<div class="container">
			<div class="credits__inner">
				<ul class="credits__inner-list">
					<li class="credits__inner-list-item">
						<div class="credits__inner-list-item-picture">
							<img src="../public/image/clock.svg" alt="#" />
						</div>
						<div class="credits__inner-list-item-info">
							<h3>Быстрая доставка</h3>
							<p>Доставим бесплатно <br>от 2000 ₽ по всей России</p>
						</div>
					</li>
					<li class="credits__inner-list-item">
						<div class="credits__inner-list-item-picture">
							<img src="../public/image/card.svg" alt="#" />
						</div>
						<div class="credits__inner-list-item-info">
							<h3>Безопасная оплата</h3>
							<p>Плати безопасно и легко <br>онлайн на нашем сайте.</p>
						</div>
					</li>
					<li class="credits__inner-list-item">
						<div class="credits__inner-list-item-picture">
							<img src="../public/image/bigStar.svg" alt="#" />
						</div>
						<div class="credits__inner-list-item-info">
							<h3>Бонусная программа</h3>
							<p>Дополнительная скидка <br>15% при регистрации</p>
						</div>
					</li>
					<li class="credits__inner-list-item">
						<div class="credits__inner-list-item-picture">
							<img src="../public/image/shoppingCart.svg" alt="#" />
						</div>
						<div class="credits__inner-list-item-info">
							<h3>Большой выбор</h3>
							<p>Ежегодно выходит в свет <br> более 100 книг</p>
						</div>
					</li>
				</ul>
			</div>
		</div>
	</section>
</template>

<style>
.credits {
    padding-bottom: 30px;
    background-color: #F9F9FA;
    padding-top: 30px;
}

.credits__inner-list {
	display: flex;
	justify-content: space-between;
}

.credits__inner-list-item {
	max-width: 290px;
	max-height: 150px;
	display: flex;
	padding: 42px 10px;
	align-items: center;
	border-radius: 5px;
	background-color: #fff;
}

.credits__inner-list-item-info p {
	font-size: 12px;
	color: rgba(114, 114, 114, 1);
}

.credits__inner-list-item-info h3 {
	font-weight: 700;
	margin-bottom: 3px;
	color: rgba(28, 41, 77, 1);
}

@media (max-width: 890px) {
    .credits{
        padding: 10px 0;
    }
	.credits__inner-list {
		flex-direction: column;
		gap: 10px;
	}

	.credits__inner-list-item {
		max-width: 375px;
		justify-content: center;
	}

	.credits__inner-list-item:nth-child(2) {
		order: 2;
	}
	.credits__inner-list-item-info p {
		max-width: 210px;
		font-size: 14px;
	}
	.credits__inner-list-item-picture img {
		width: 90px;
	}
}
</style>
