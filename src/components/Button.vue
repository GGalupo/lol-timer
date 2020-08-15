<template>
    <button class="button">{{ label }}</button>
</template>

<script>
export default {
	props: ['label']
}
</script>

<style>
.button {
	box-shadow: 3px 2px 0px 0px #899599;
	background:linear-gradient(to bottom, #c7d7ff 5%, #ebe0ca 100%);
	background-color:#c7d7ff;
	border-radius:9px;
	border:1px solid #e8dae8;
	display:inline-block;
	cursor:pointer;
	color:#e64949e7;
	font-family:Trebuchet MS;
	font-size: 0.9em;
	font-weight:bold;
	/* font-style:italic; */
	padding:8px 18px;
	text-decoration:none;
	text-shadow:0px 1px 0px #e1e2ed;
	outline: none;
}
.button:hover {
	background:linear-gradient(to bottom, #ebe0ca 5%, #c7d7ff 100%);
	background-color:#ebe0ca;
}
.button:active {
	position:relative;
	top:1px;
}
</style>