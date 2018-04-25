# sanju
hi hello...ester..
print("Helloworld")
<!DOCTYPE>
<html>
	<head>
		<meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=0.1, maximum-scale=1.0">
		<script src="libs/jquery.js" type="text/javascript"></script>
		<script src="libs/jquery.tmpl.min.js" type="text/javascript"></script>
		<script src="libs/jquery-ui.min.js" type="text/javascript"></script>
		<link href="libs/jquery-ui.min.css" rel="stylesheet"></link>
		<script src=”UI/libs/jquery.js” type=”text/javascript”></script>
		<script src=”UI/libs/jquery.tmpl.min.js” type=”text/javascript”></script>
		<script src=”UI/libs/jquery-ui.min.js” type=”text/javascript”></script>
		<link href=”UI/libs/jquery-ui.min.css” rel=”stylesheet”></link>
		<script src=”UI/chatWindow.js” type=”text/javascript”></script>
		<link href=”UI/chatWindow.css” rel=”stylesheet”></link>
		“clientSecret”: “< nOOfZxxnaJHTi8ZkIQtbJU29279D8y4ESVWgB2nHCjs= >”
		$.ajax({
		url: “http://localhost:3000/api/users/sts”,
		<script src="../libs/lodash.min.js"></script>
		<script src='../libs/anonymousassertion.js'></script>
		<script src="../kore-bot-sdk-client.js"></script>
		<script src="chatWindow.js" type="text/javascript"></script>
		<script src="../libs/emoji.js" type="text/javascript"></script>
		<script src="../libs/recorder.js" type="text/javascript"></script>
		<script src="../libs/recorderWorker.js" type="text/javascript"></script>
		<link href="chatWindow.css" rel="stylesheet"></link>
		<link href="../libs/emojione.sprites.css" rel="stylesheet"></link>
		<link href="../libs/purejscarousel.css" rel="stylesheet"></link>
		<script src="../libs/purejscarousel.js" type="text/javascript"></script>
		<script src="custom/customTemplate.js" type="text/javascript"></script>
		<link href="custom/customTemplate.css" rel="stylesheet"></link>
		<script type="text/javascript" src="libs/loader.js"></script>
		<script type="text/javascript" src="../libs/speech/app.js"></script>
		<script type="text/javascript" src="../libs/speech/key.js"></script>
		<script type="text/javascript" src="../libs/client_api.js"></script>
		<script type="text/javascript">
			$(document).on("ready", function () {
				function assertion(options, callback) {
					var jsonData = {
						"clientId": botOptions.clientId,
						"clientSecret": "",
						"identity": botOptions.userIdentity,
						"aud": "",
						"isAnonymous": false
					};
					$.ajax({
						url: botOptions.koreAPIUrl + "users/sts",
						type: 'post',
						data: jsonData,
						dataType: 'json',
						success: function (data) {
							options.assertion = data.jwt;
							options.handleError = koreBot.showError;
							options.chatHistory = koreBot.chatHistory;
							options.botDetails = koreBot.botDetails;
							callback(null, options);
							setTimeout(function () {
								if (koreBot && koreBot.initToken) {
									koreBot.initToken(options);
								}
							}, 2000);
						},
						error: function (err) {
							koreBot.showError(err.responseText);
						}
					});
				}

</html>
