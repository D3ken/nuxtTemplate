<script setup>

</script>

<template>
	<section class="news">
		<div class="container">
			<div class="news__inner">
				<div class="news__inner-heading">
					<h3>Новости</h3>
					<div class="news__inner-heading-btns">
						<div class="btn-left block-header-arrows">
                            <img src="../public/image/leftArrow.svg" alt="#">
                        </div>
                        <div class="btn-right block-header-arrows">
                            <img src="../public/image/rightArrow.svg" alt="#">
                        </div>
					</div>
				</div>
				<ul class="news__inner-list">
					<li class="news__inner-list-item">
						<div class="news__inner-list-item-picture">
							<img src="../public/image/newsImg1.svg" alt="#" />
						</div>
						<div class="news__inner-list-item-description">
							<p>16 июня 2020</p>
							<p>
								Бесплатный онлайн-семинар. Доктрина stare decisis: борьба за
								прецедент в рос...
							</p>
							<p>
								18 июня в «Клубе цивилистов» пройдет бесплатный онлайн-семинар
								по проблематике судебного прецедента. Мероприятие приуроч...
							</p>
						</div>
						<div class="news__inner-list-item-read-btn">
							<button><span>Читать</span></button>
						</div>
					</li>
					<li class="news__inner-list-item">
						<div class="news__inner-list-item-picture">
							<img src="../public/image/newsImg2.svg" alt="#" />
						</div>
						<div class="news__inner-list-item-description">
							<p>16 июня 2020</p>
							<p>
								Бесплатный онлайн-семинар. Доктрина stare decisis: борьба за
								прецедент в рос...
							</p>
							<p>
								18 июня в «Клубе цивилистов» пройдет бесплатный онлайн-семинар
								по проблематике судебного прецедента. Мероприятие приуроч...
							</p>
						</div>
						<div class="news__inner-list-item-read-btn">
							<button><span>Читать</span></button>
						</div>
					</li>
					<li class="news__inner-list-item">
						<div class="news__inner-list-item-picture">
							<img src="../public/image/newsImg3.svg" alt="#S" />
						</div>
						<div class="news__inner-list-item-description">
							<p>16 июня 2020</p>
							<p>
								Бесплатный онлайн-семинар. Доктрина stare decisis: борьба за
								прецедент в рос...
							</p>
							<p>
								18 июня в «Клубе цивилистов» пройдет бесплатный онлайн-семинар
								по проблематике судебного прецедента. Мероприятие приуроч...
							</p>
						</div>
						<div class="news__inner-list-item-read-btn">
							<button><span>Читать</span></button>
						</div>
					</li>
				</ul>
				<div class="news__inner-all">
					<a href="">Показать все новости</a>
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
.news {
	padding-bottom: 30px;
    padding-top: 30px;
    background-color: #F9F9FA;
}

.news__inner-heading {
	display: flex;
	align-items: center;
	justify-content: space-between;
	padding: 18px 25px;
}

.news__inner-heading-btns{
    display: flex;
}

.news__inner {
	background-color: rgba(255, 255, 255, 1);
	border-radius: 5px;
}

.news__inner-heading h3 {
	font-size: 20px;
	font-weight: 700;
	color: rgba(28, 41, 77, 1);
}

.news__inner-list {
	border-top: 1px solid rgba(28, 41, 77, 0.15);
}
.news__inner-all {
	display: none;
}
.news__inner-list-item {
	padding: 25px 20px;
}

.news__inner-list-item-picture {
	margin-bottom: 15px;
}

.news__inner-list-item-description {
	max-width: 320px;
}

.news__inner-list-item-description p:first-child {
	font-size: 12px;
	font-weight: 400;
	color: rgba(28, 41, 77, 0.5);
	margin-bottom: 5px;
}

.news__inner-list-item-description p:nth-child(2) {
	color: rgba(28, 41, 77, 1);
	font-weight: 600;
	font-size: 16px;
	margin-bottom: 8px;
}

.news__inner-list-item-description p:last-child {
	margin-bottom: 12px;
}
.news__inner-list-item-picture img {
	border-radius: 5px;
}

.news__inner-list-item-read-btn button {
	background-color: transparent;
	padding: 10px 67px;
	border: 1px solid rgba(28, 41, 77, 0.15);
}

.news__inner-list-item-read-btn button span {
	font-weight: 600;
	font-size: var(--text-main-size);
}

.news__inner-list {
	display: flex;
	justify-content: space-between;
}

.news__inner-list-item:nth-child(2) {
	border-left: 1px solid rgba(28, 41, 77, 0.15);
	border-right: 1px solid rgba(28, 41, 77, 0.15);
}


@media (max-width: 890px) {
	.news__inner-list-item:nth-child(2) {
		display: none;
	}
	.news__inner-list-item-read-btn button {
		width: 100%;
	}
	.news__inner-list-item:last-child {
		display: none;
	}
	.news__inner-list {
		align-items: center;
		flex-direction: column;
		border-bottom: 1px solid rgba(28, 41, 77, 0.15);
	}
	.news__inner-all {
		display: block;
		text-align: center;
		padding: 10px 0px;
	}

	.news__inner-all a {
		font-size: 14px;
		font-weight: 600;
	}
}
</style>
