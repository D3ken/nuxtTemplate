<script setup>

</script>

<template>
	<section class="released">
		<div class="container">
			<div class="released__inner">
				<div class="released__inner-heading">
					<h3>Готовяться к выходу</h3>
					<div class="released__inner-heading-btn">
						<div class="btn-left block-header-arrows">
                            <img src="../public/image/leftArrow.svg" alt="#">
                        </div>
                        <div class="btn-right block-header-arrows">
                            <img src="../public/image/rightArrow.svg" alt="#">
                        </div>
					</div>
				</div>
				<ul class="released__inner-list">
					<li class="released__inner-list-item">
						<div class="released__inner-list-item-picture">
							<img src="../public/image/book1.png" alt="#" />
						</div>
						<div class="released__inner-list-item-description">
							<p>Корпоративное право</p>
							<p>
								Инвестирование: способы,<br />
								риски, субъекты : монография
							</p>
							<p>Майфат А.В.</p>
							<p>4 450 ₽</p>
						</div>
						<div class="released__inner-list-item-rating">
							<p class="star">
								<img src="../public/image/starIcon.svg" alt="#" /><span>4.9</span>
							</p>
							<p class="rec">
								<img src="../public/image/likeIcon.svg" alt="#" /><span>89% рекомендуют</span>
							</p>
						</div>
						<div class="released__inner-list-item-btns">
							<button>
								<img src="../public/image/orangeCart.svg" alt="#" />
								<span>В корзину</span>
							</button>
							<button>
								<img src="../public/image/laterIcon.svg" alt="#" />
							</button>
						</div>
					</li>
					<li class="released__inner-list-item">
						<div class="released__inner-list-item-picture">
							<img src="../public/image/book2.png" alt="#" />
						</div>
						<div class="released__inner-list-item-description">
							<p>Корпоративное право</p>
							<p>
								Договор коммерческой<br />
								концессии (франчайзинг). Граж...
							</p>
							<p>Майфат А.В.</p>
							<p>4 450 ₽</p>
						</div>
						<div class="released__inner-list-item-rating">
							<p class="star">
								<img src="../public/image/starIcon.svg" alt="#" /><span>4.9</span>
							</p>
							<p class="rec">
								<img src="../public/image/likeIcon.svg" alt="#" /><span>89% рекомендуют</span>
							</p>
						</div>
						<div class="released__inner-list-item-btns">
							<button>
								<img src="../public/image/orangeCart.svg" alt="#" />
								<span>В корзину</span>
							</button>
							<button>
								<img src="../public/image/laterIcon.svg" alt="#" />
							</button>
						</div>
					</li>
					<li class="released__inner-list-item">
						<div class="released__inner-list-item-picture">
							<img src="../public/image/book3.png" alt="#" />
						</div>
						<div class="released__inner-list-item-description">
							<p>Корпоративное право</p>
							<p>
								Договор коммерческой<br />
								концессии (франчайзинг). Граж...
							</p>
							<p>Майфат А.В.</p>
							<p class="price-history">
								<span class="actual-price">4 450 ₽ </span
								><span class="old-price"
									>1 284 ₽ <img src="../public/image/redline.svg" alt="#"
								/></span>
								<span class="profit">Выгода 300 ₽</span>
							</p>
						</div>
						<div class="released__inner-list-item-rating">
							<p class="star">
								<img src="../public/image/starIcon.svg" alt="#" /><span>4.9</span>
							</p>
							<p class="rec">
								<img src="../public/image/likeIcon.svg" alt="#" /><span>89% рекомендуют</span>
							</p>
						</div>
						<div class="released__inner-list-item-btns">
							<button>
								<img src="../public/image/orangeCart.svg" alt="#" />
								<span>В корзину</span>
							</button>
							<button>
								<img src="../public/image/laterIcon.svg" alt="#" />
							</button>
						</div>
					</li>
					<li class="released__inner-list-item">
						<div class="released__inner-list-item-picture">
							<img src="../public/image/book1.png" alt="#" />
						</div>
						<div class="released__inner-list-item-description">
							<p>Корпоративное право</p>
							<p>
								Инвестирование: способы,<br />
								риски, субъекты : монография
							</p>
							<p>Майфат А.В.</p>
							<p>4 450 ₽</p>
						</div>
						<div class="released__inner-list-item-rating">
							<p class="star">
								<img src="../public/image/starIcon.svg" alt="#" /><span>4.9</span>
							</p>
							<p class="rec">
								<img src="../public/image/likeIcon.svg" alt="#" /><span>89% рекомендуют</span>
							</p>
						</div>
						<div class="released__inner-list-item-btns">
							<button>
								<img src="../public/image/orangeCart.svg" alt="#" />
								<span>В корзину</span>
							</button>
							<button>
								<img src="../public/image/laterIcon.svg" alt="#" />
							</button>
						</div>
					</li>
				</ul>
				<div class="released__inner-list-all">
					<a href="#">Показать все книги раздела</a>
				</div>
			</div>
		</div>
	</section>
</template>

<style>
.block-header-arrows{
    padding: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    border: 1px solid #1C294D26;
    cursor: pointer;
}
.btn-right{
    border-radius: 0 5px 5px 0;
    border-left: none;
}
.btn-left{
    border-radius: 5px 0 0 5px;
}
.released__inner {
	background-color: #fff;
	border-radius: 5px;
}
.released__inner-heading {
	display: flex;
	justify-content: space-between;
	align-items: center;
	padding: 18px 25px;
}
.released__inner-heading h3 {
	font-size: 20px;
	font-weight: 700;
}
.released__inner-heading-btn {
	display: flex;
	width: 60px;
	height: 30px;
}

.released__inner-heading-btn button img {
	width: 60px;
	height: 30px;
}

.released__inner-list {
	border-top: 1px solid rgba(28, 41, 77, 0.15);
	border-bottom: 1px solid rgba(28, 41, 77, 0.15);
	display: flex;
	justify-content: space-between;
}

.released__inner-list-item {
	display: flex;
	flex-direction: column;
	/* padding: 20px 60px; */
	padding-bottom: 21px;
	max-width: 288px;
}

.released__inner-list-item-description {
	padding-left: 20px;
	max-width: 320px;
	font-size: 12px;
	margin-bottom: 10px;
}

.released__inner-list-item-picture {
	padding: 25px 60px 0px 60px;
	align-self: center;
	margin-bottom: 15px;
}

.released__inner-list-item:nth-child(2) {
	border-left: 1px solid rgba(28, 41, 77, 0.15);
	border-right: 1px solid rgba(28, 41, 77, 0.15);
}

.released__inner-list-item:nth-child(4) {
	border-left: 1px solid rgba(28, 41, 77, 0.15);
}

.released__inner-list-item-description p:first-child {
	font-weight: 400;
	margin-bottom: 8px;
	color: rgba(28, 41, 77, 0.5);
}

.released__inner-list-item p:nth-child(2) {
	font-weight: 600;
	font-size: 14px;
	margin-bottom: 8px;
	color: rgba(28, 41, 77, 1);
}

.released__inner-list-item p:nth-child(3) {
	font-weight: 400;
	font-size: 14px;
	color: rgba(28, 41, 77, 0.5);
	margin-bottom: 8px;
}

.released__inner-list-item p:last-child {
	font-weight: 600;
	font-size: 18px;
	color: rgba(28, 41, 77, 1);
}

.released__inner-list-item-btns {
	display: flex;
	align-items: center;
	justify-content: center;
	gap: 10px;
}

.released__inner-list-item-btns button {
	display: flex;
	align-items: center;
	gap: 10px;
	background-color: #fff;
	border: 1px solid rgba(238, 238, 238, 1);
	border-radius: 5px;
}

.released__inner-list-item-btns button img:last-child {
	padding: 10px 15px;
}

.released__inner-list-item-btns button:first-child {
	padding: 10px 25px;
}

.released__inner-list-all {
	text-align: center;
    padding: 18px 0;
}

.released__inner-list-item-rating {
	display: flex;
	align-items: center;
	gap: 10px;
	padding-left: 20px;
}

.released__inner-list-item-rating p {
	display: flex;
	gap: 3px;

	border-radius: 5px;
}

.star {
	padding: 5px 8px;
	font-weight: 600;
	background-color: rgba(251, 192, 45, 0.3);
}

.rec {
	display: flex;
	gap: 5px;
	padding: 5px 10px;
	font-weight: 600;
	background-color: rgba(121, 134, 203, 0.3);
}

.rec span {
	color: rgba(121, 134, 203, 1);
    font-size: 12px;
}

.star span {
	color: rgba(251, 192, 45, 1);
    font-size: 12px;
}

.actual-price {
	color: rgba(253, 58, 58, 1);
	font-size: 18px;
	font-weight: 700;
}

.old-price {
	position: relative;
	color: rgba(28, 41, 77, 0.5);
	font-size: 12px;
}

.old-price img {
	position: absolute;
	top: 25%;
	left: 0;
}

.profit {
	color: rgba(13, 185, 140, 1);
	font-size: 12px;
}

.released__inner-list-item-btns button span {
	font-size: 14px;
	font-weight: 600;
}

.price-history {
	display: flex;
	align-items: center;
	gap: 7px;
}

@media (max-width: 890px) {
	.released__inner-list-item:nth-child(3) {
		display: none;
	}

	.released__inner-list-item:nth-child(2) {
		display: none;
	}

	.released__inner-list-item {
		max-width: 170px;
		margin-left: 10px;
	}

	.released__inner-list-item-picture {
		padding: 20px 25px 0px 0px;
		margin-left: 25px;
		align-self: auto;
	}

	.released__inner-list-item-picture img {
		max-width: 126px;
	}

	.released__inner-list-item-description {
		padding-left: 10px;
	}

	.released__inner-list-item-rating {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		padding-left: 10px;
	}

	.rec {
		padding: 6px 10px;
        width: 100%;
	}

	.rec span {
		font-size: 12px;
	}
	.released__inner-list {
		justify-content: unset;
	}
	.star span {
		font-size: 12px;
	}
	.released__inner-list-item-btns {
		padding-left: 10px;
	}

	.released__inner-list-item-btns button {
		height: 35px;
	}
	.released__inner-list-item-btns button:first-child {
		padding: 10px 13px;
	}
	.released__inner-list-item-btns button img:last-child {
		padding: 10px 12px;
	}
	.released__inner-list-item-btns button span {
		font-size: 9px;
	}
	.released__inner-list {
		margin-bottom: 0px;
	}
	.released__inner-list-all {
		padding: 10px 0px;
		font-size: 14px;
		font-weight: 600;
		color: rgba(28, 41, 77, 1);
	}
	.released__inner-list-item:last-child .released__inner-list-item-rating .rec {
		visibility: hidden;
	}
}
</style>
