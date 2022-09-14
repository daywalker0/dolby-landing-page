<template>
	<div class="form__container">
		<h1 class="form__title title">Never Miss a drop!</h1>
		<p class="form__subtitle subtitle">Subscribe to our ultra-exclusive drop list and be the first to know about upcoming dolby drops.</p>
		<form class="subscribe-form-form" action="#">
			<label for="email"></label>
			<input
				name="email"
				class="email-input"
				type="text"
				placeholder="Email Address"
				v-model.trim="email"
				@input="inputValue = $event.target.value">
			<button
				class="btn-submit-form"
				type="submit">Subscribe</button>
		</form>
	</div>
</template>

<script>
export default {
	data() {
		return {
			email: '',
		}
	},
	methods: {
		submitForm: function() {}
	},
}
</script>

<style lang="scss" scoped>
.form {
	&__container {
		text-align: center;
	}
	&__title {
		font-size: 48px;
		line-height: 62px;
	}
	&__subtitle {
		max-width: 714px;
		margin: 0 auto;
		padding: 6px 0 39px;
	}
}
.subtitle {
}

.subscribe-form-form {
	display: flex;
	max-width: 700px;
	margin: 0 auto;
}
.email-input {
	padding: 26px 379px 26px 40px;
	background: none;
	border: 1px solid #FFFFFF;
	filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
	border-top-left-radius: 50px;
	border-bottom-left-radius: 50px;
	border-right: none;
	color: #fff;
	font-size: 18px;
	&::placeholder {
		font-family: Poppins;
		font-weight: 400;
		font-size: 18px;
		line-height: 28px;
		color: rgba(255, 255, 255, 0.5);
	}
	&:focus:-ms-input-placeholder { color:transparent; } /* IE 10+ */
	&:focus::-webkit-input-placeholder { color:transparent; }
	&:focus:-moz-placeholder { color:transparent; } /* FF 4-18 */
	&:focus::-moz-placeholder { color:transparent; } /* FF 19+ */

}
.btn-submit-form {
	padding: 26px 31px;
	background: #FFFFFF;
	border: 1px solid #FFFFFF;
	box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
	border-radius: 50px;
	margin-left: -35px;
	justify-self: flex-end;
	cursor: pointer;
	font-family: Poppins;
	font-weight: 600;
	font-size: 18px;
	line-height: 28px;
	text-align: center;
	color: rgba(0, 0, 0, 0.75);
}
</style>