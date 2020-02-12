function validation() {
	var name = document.getElementById("name").value;
	var password = document.getElementById("password").value;
	var email = document.getElementById("email").value;
	var confirm = document.getElementById("confirm").value;

	if(name == '' ){
		document.getElementById("messages").innerHTML="** Please Fill the Student Number";
		return true;
	}	

	if(email == '' ){
		document.getElementById("messages1").innerHTML="** Please Fill the email";
		return false;
	}

	if(password == '' ) {
		document.getElementById("messages2").innerHTML="** Please Fill the password";
		return false;
	}

	if(password.length <= 5) {
		document.getElementById("messages2").innerHTML="** Password must be greater than 5";
		return false;
	}

	if(password.length > 25) {
		document.getElementById("messages2").innerHTML="** Password must be less than 25";
		return false;
	}

	if(confirm == '' ) {
		document.getElementById("messages3").innerHTML="** Please re-enter your password";
		return false;
	}

	if(password!=confirm) {
		document.getElementById("messages3").innerHTML="** Password does not match";
		return false;
	}
}

const errorElement = document.getElementById('error')
form.addEventListener('submit', (e) => {
	
		e.preventDefault()
	}
)