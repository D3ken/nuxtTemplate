<script setup>

</script>

<template>
	<footer class="footer">
		<div class="container">
			<div class="footer__inner">
				<ul class="footer__inner-list">
					<li class="heading">
						<h3><a href="#">Покупателям</a></h3>
					</li>
					<li><a href="#">Наша почта</a></li>
					<li><a href="#">Оплата и доставка</a></li>
					<li><a href="#">Вопросы и ответы</a></li>
				</ul>
				<ul class="footer__inner-list">
					<li class="heading">
						<h3><a href="#">Издательство</a></h3>
					</li>
					<li><a href="#">О компании</a></li>
					<li><a href="#">Авторам</a></li>
					<li><a href="#">Вакансии</a></li>
					<li><a href="#">Контакты</a></li>
				</ul>
				<ul class="footer__inner-list">
					<li class="heading">
						<h3><a href="#">Книги</a></h3>
					</li>
					<li><a href="#">Все категории</a></li>
					<li><a href="#">Бестселлеры</a></li>
					<li><a href="#">Новинки</a></li>
					<li><a href="#">Скидки и акции</a></li>
				</ul>
				<ul class="footer__inner-list">
					<li class="heading">
						<h3><a href="#">Прайс-лист</a></h3>
					</li>
					<li>
						<p class="price-list">
							<img src="../public/image/fileIcon.svg" alt="#" />
							<span
								>Скачать прайс-лист<br />
								<span class="not-bright">PDF, 12 Mb </span></span
							>
						</p>
					</li>
				</ul>
				<ul class="footer__inner-list">
					<li class="heading">
						<h3><a href="#">Телефон и Email</a></h3>
					</li>
					<li>
						<p class="tel">
							<img src="../public/image/mail.svg" alt="#" />
							<span>market@estatut.ru</span>
						</p>
					</li>

					<li>
						<p class="tel">
							<img src="../public/image/phone.svg" alt="#" />
							<span>8 (968) 660-65-50</span>
						</p>
					</li>
				</ul>
			</div>
			<div class="footer__credentials">
				<p>© 2020 Издательство «Статут»</p>
				<ul>
					<li>
						<a href="">ул. Лобачевского, 92, корп. 2 119454, г. Москва</a>
					</li>
					<li><a href="">Политика конфиденциальности</a></li>
					<li><a href="">Договор оферты</a></li>
				</ul>
			</div>

			<div class="footer__credentials-media">
				<ul>
					<li class="footer-link">
						<p>Покупателям</p>
						<img src="../public/image/downArrow.svg" alt="#" />
					</li>
					<li class="footer-link">
						<p>Издательство</p>
						<img src="../public/image/downArrow.svg" alt="#" />
					</li>
					<li class="footer-link">
						<p>Книги</p>
						<img src="../public/image/downArrow.svg" alt="#" />
					</li>
					<li class="footer-link">
						<p>Прайс-лист</p>
						<img src="../public/image/downArrow.svg" alt="#" />
					</li>
				</ul>
			</div>
		</div>
	</footer>
	<div class="polytics">
		<div class="container">
			<div class="polytics__inner">
				<ul>
					<li>
						<p>Политика конфиденциальности</p>
						<p>Договор оферты</p>
					</li>
					<li class="footer-img-link">
						<img src="../public/image/phone.svg" alt="#" />
						<span>8 (968) 660-65-50</span>
						<img src="../public/image/info.svg" alt="#" />
					</li>
					<li class="footer-img-link">
						<img src="../public/image/mail.svg" alt="#" />
						<span>market@estatut.ru</span>
					</li>
					<li class="footer-img-link">
						<img src="../public/image/location.svg" alt="#" />
						<span>ул. Лобачевского, 92, корп. 2 119454, г. Москва</span>
					</li>
				</ul>
			</div>
		</div>
	</div>
	<div class="copyright">
		<div class="container">
			<div class="p">© 2020 Издательство «Статут»</div>
		</div>
	</div>
</template>

<style>
/* FOOTER START */

.footer {
	background-color: #fff;
}

.footer__inner {
	padding: 45px 0px;
	border-bottom: 1px solid rgba(40, 47, 54, 0.15);
}
.heading {
	margin-bottom: 25px;
}
.footer__inner-list {
	display: flex;
	flex-direction: column;
	align-items: flex-start;
}
.footer__inner-list li:not(:first-child) {
	margin-bottom: 15px;
}

.price-list {
	display: flex;
	align-items: center;
	gap: 5px;
}

.not-bright {
	color: rgba(40, 47, 54, 0.5);
	font-size: 12px;
}

.footer__inner {
	display: flex;
	gap: 70px;
}

.tel {
	display: flex;
	gap: 5px;
	align-items: center;
}

.footer__credentials {
	display: flex;
	justify-content: space-between;
	padding: 40px 0px 45px 0px;
}

.footer__credentials ul {
	display: flex;
}

.footer__credentials ul li:first-child {
	margin-right: 67px;
}

.footer__credentials p {
	color: rgba(28, 41, 77, 0.5);
}

.footer__credentials ul li:nth-child(2) {
	margin-right: 30px;
}
.footer__credentials-media {
	display: none;
}
.polytics {
	display: none;
}
.copyright {
	display: none;
}


@media (max-width: 890px) {
	.footer__inner {
		display: none;
	}

	.polytics {
		display: block;
		border-bottom: 1px solid rgba(42, 61, 72, 0.15);
	}
	.footer__credentials {
		display: none;
	}

	.footer__credentials-media {
		display: flex;
		flex-direction: column;
        width: 90%;
	}

	.footer-link {
		padding: 20px 0px;
		display: flex;
		align-items: center;
        text-align: center;
		justify-content: space-between;
		color: rgba(42, 61, 72, 1);
		font-weight: 500;
	}

	.footer-link:not(:last-child) {
		border-bottom: 1px solid rgba(42, 61, 72, 0.15);
		padding-bottom: 20px;
	}
	.footer {
		border-bottom: 1px solid rgba(42, 61, 72, 0.15);
	}
	.polytics {
		background-color: #fff;
	}
	.polytics__inner {
		padding: 20px 0px 0px 0px;
	}
	.polytics__inner ul li {
		padding: 20px 20px;
		border-bottom: 1px solid rgba(42, 61, 72, 0.15);
	}
	.polytics__inner ul li:first-child {
		color: rgba(28, 41, 77, 0.5);
	}
	.footer-img-link {
		display: flex;
		align-items: center;
		gap: 5px;
	}

	.footer-img-link:last-child {
		border-bottom: none;
	}
	.copyright {
		display: block;
		padding: 20px 0px;
		background-color: #fff;
	}

	.p {
		color: rgba(28, 41, 77, 0.5);
	}
}
</style>
