<script setup>

</script>

<template>
	<section class="mailBlock">
		<div class="container">
			<div class="mailBlock__inner">
				<p class="rel one">
					<span>Скидка 200 ₽ при подписке на рассылку Издательства</span>
					<img src="./img/orange-line-small.svg" alt="" />
				</p>
				<p class="rel two">
					<span
						>Скидка 200 ₽ при подписке <br />
						на рассылку Издательства</span
					>
					<img src="./img/orange-line-small.svg" alt="" />
				</p>

				<input placeholder="Введите ваш Email" type="text" />
				<button><span>Подписаться</span></button>
			</div>
		</div>
	</section>
</template>

<style>
.mailBlock {
	padding-bottom: 30px;
    background-color: #F9F9FA;
    padding-top: 30px;
}
.mailBlock__inner {
	background-color: rgba(2, 136, 209, 1);
	border-radius: 5px;
	padding: 42px 45px;
	display: flex;
	position: relative;
	align-items: center;
	max-height: 105px;
}

.mailBlock__inner input {
	margin-right: 10px;
	padding: 10px 15px;
	width: 418px;
	border-radius: 5px;
	border: none;
}

.mailBlock__inner button {
	padding: 10px 25px;
	background-color: transparent;
	border: 1px solid rgba(255, 255, 255, 1);
	border-radius: 5px;
}

.mailBlock__inner button span {
	color: rgba(255, 255, 255, 1);
	font-size: 14px;
	font-weight: 600;
}

.mailBlock__inner p span {
	color: rgba(255, 255, 255, 1);
	font-weight: 700;
	font-size: 16px;
	margin-right: 14px;
}
.rel span {
	position: relative;
	z-index: 100;
}
.mailBlock__inner p img {
	width: 52px;
	z-index: 1;
	position: absolute;
	left: 9%;
	top: 36%;
}
.one{
    margin-bottom: 0px;
}
.two {
	display: none;
}

@media (max-width: 890px) {
	.mailBlock__inner {
		display: flex;
		flex-direction: column;
		max-height: 100%;
		gap: 10px;
		padding: 20px 10px;
        max-width: 95%;
	}

	.mailBlock__inner input {
		max-width: 100%;
	}
	.mailBlock__inner input {
		margin-right: 0px;
	}

	.mailBlock__inner button {
		width: 100%;
	}

	.mailBlock__inner p img {
		left: 17%;
		top: 10%;
	}

	.one {
		display: none;
	}

	.two {
		display: block;
		align-self: flex-start;
	}
	.mailBlock {
		padding-bottom: 10px;
        padding-top: 10px;
	}
}

</style>
