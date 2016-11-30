<?php
//Contact form stuff
    function test_input($data)
	{
		$data = trim($data);
		$data = stripslashes($data);
		$data = htmlspecialchars($data);
		return $data;
	}
	
	if(isset($_POST['submit'])):
	if(isset($_POST['g-recaptcha-response']) && !empty($_POST['g-recaptcha-response'])):
	$secret = 'YOUR SECRET KEY GOES HERE';
	$verifyResponse = file_get_contents('https://www.google.com/recaptcha/api/siteverify?secret='.$secret.'&response='.$_POST['g-recaptcha-response']);
	$responseData = json_decode($verifyResponse);
	$contact_name = !empty($_POST['contact_name'])?$_POST['contact_name']:'';
	$contact_name = test_input($contact_name);
	$email = !empty($_POST['email'])?$_POST['email']:'';
	$email = test_input($email);
	$tel_no = !empty($_POST['tel_no'])?$_POST['tel_no']:'';
	$tel_no = test_input($tel_no);
	$con_website = !empty($_POST['con_website'])?$_POST['con_website']:'';
	$con_website = test_input($con_website);
	$message = !empty($_POST['message'])?$_POST['message']:'';
	//Make sure the email address is valid
	if (preg_match("/([\w\-]+\@[\w\-]+\.[\w\-]+)/",$email)):
	$email = $email;
	if($responseData->success):
	//contact form submission code
	$to = "YOUR EMAIL ADDRESS HERE";
	$subject = "Contact form submission from ".$contact_name."";
	$htmlContent = "
		<p><b>Name: </b>".$contact_name."</p>
		<p><b>Email Address: </b>".$email."</p>
		<p><b>Phone Number: </b>".$tel_no."</p>
		<p><b>Website Address: </b>".$con_website."</p>
		<p><b>Message: </b>".$message."</p>";
	//Set the content type for sending HTML email
	$headers = "MIME-Version: 1.0" . "\r\n";
	$headers .= "Content-type:text/html;charset=UTF-8" . "\r\n";
	$headers .= 'From:'.$contact_name.' <'.$email.'>' . "\r\n";
	//Send the message
	@mail($to, $subject,$htmlContent,$headers);
	$succMsg = '
				<div class="alert alert-success alert-dismissible" role="alert">
                    <button type="button" class="close" data-dismiss="alert" aria-label="Close"><span aria-hidden="true">&times;</span></button>
					Your message has been sent.  Someone will be in touch shortly.
				</div>
			';
	$contact_name = '' ;
	$email = '' ;
	$tel_no = '' ;
	$con_website = '' ;
	$message = '' ;
	else: 
		$errMsg = '
					<div class="alert alert-danger alert-dismissible" role="alert">
            			<button type="button" class="close" data-dismiss="alert" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            			Captcha failed, please try again.
            		</div>
            	';
	endif;
	else: 
		$errMsg = '
					<div class="alert alert-danger alert-dismissible" role="alert">
                        <button type="button" class="close" data-dismiss="alert" aria-label="Close"><span aria-hidden="true">&times;</span></button>
						There is a problem with your email address, please check and re-type.
					</div>
				';
	endif;
	else: 
		//Re-display content if error
		$contact_name = $_POST['contact_name']; 
		$email = $_POST['email'];
		$tel_no = $_POST['tel_no'];
		$con_website = $_POST['con_website'];
		$message = $_POST['message'];
		$errMsg = 'Please click on the reCaptcha "I\'m not a robot" box.';
	endif;
	else: 
		$errMsg = '';
		$succMsg = '';
		$contact_name = '';
		$email = '';
		$tel_no = '';
		$con_website = '';
		$message = '';
	endif;
?>

<!doctype html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
        <title>365-Tech</title>
        <meta name="description" content="">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        
        <!-- link the stylesheets -->
        <link rel="stylesheet" href="style.css">
		
		<!-- Google Font -->
		<link href="https://fonts.googleapis.com/css?family=Orbitron" rel="stylesheet">
        

        <!-- link Google captcha api -->
        <script src="https://www.google.com/recaptcha/api.js"></script>
        

        <!-- Meta & OG Stuff -->
        <meta property="og:image" content=""><!-- your logo -->
        <meta property="og:title" content=""><!-- your site title -->
        <meta property="og:url" content=""><!-- your site url -->
        <meta property="og:site_name" content=""><!-- your site name -->
        <meta name="keywords" content=" "><!-- keywords for your site -->
        <meta name="description" content=""><!-- your site description -->

    </head>
    <body>
		<header>
			<div class="row">
				<div class="container">
					<div class="col-md-6 col-md-offset-3 col-sm-12 text-center">
						<div class="well">
							<form action="" method="POST">

								<div class="form-group">
									<div class="col-md-8 col-md-offset-2 input-group">
										<span class="input-group-addon">
											<i class="fa fa-user"></i>
										</span>
										<input class="form-control" type="text" value="<?php echo !empty($contact_name)?$contact_name:'' ;?>" placeholder="Your Full Name" name="contact_name" required>
									</div><!-- closes input-group -->
								</div><!-- closes form-group -->

								<div class="form-group">
									<div class="col-md-8 col-md-offset-2 input-group">
										<span class="input-group-addon">
											<i class="fa fa-envelope"></i>
										</span>
										<input class="form-control" type="text" value="<?php echo !empty($email)?$email:''; ?>" placeholder="Your email address" name="email" required>
									</div><!-- closes input-group -->
								</div><!-- closes form-group -->

								<div class="form-group">
									<div class="col-md-8 col-md-offset-2 input-group">
										<span class="input-group-addon">
											<i class="fa fa-phone"></i>
										</span>
										<input class="form-control" type="text" value="<?php echo !empty($tel_no)?$tel_no:''; ?>" placeholder="Your phone number" name="tel_no">
									</div><!-- closes input-group -->
								</div><!-- closes form-group -->

								<div class="form-group">
									<div class="col-md-8 col-md-offset-2 input-group">
										<span class="input-group-addon">
											<i class="fa fa-globe"></i>
										</span>
										<input class="form-control" type="text" value="<?php echo !empty($con_website)?$con_website:''; ?>"
				placeholder="Your website address" name="con_website">
									</div><!-- closes input-group -->
								</div><!-- closes form-group -->

								<div class="form-group">
									<div class="col-md-8 col-md-offset-2 input-group">
										<span class="input-group-addon">
											<i class="fa fa-pencil"></i>
										</span>
										<textarea class="form-control" type="text" placeholder="Your message" name="message" rows="3" cols="4" required>
											<?php echo !empty($message)?$message:''; ?>
										</textarea>
									</div><!-- closes input-group -->
								</div><!-- closes form-group -->

								<div class="form-group">
									<div class="col-md-8 col-md-offset-2 input-group">
										<div class="g-recaptcha" data-sitekey="YOUR SITE KEY GOES HERE"></div>
									</div><!-- closes input-group -->
								</div><!-- closes form-group -->

								<div class="form-group">
									<div class="col-md-8 col-md-offset-2">
										<?php if(!empty($succMsg)): ?>
										<?php echo $succMsg; ?>
										<?php endif; ?>
										<?php if(!empty($errMsg)): ?>
										<?php echo $errMsg; ?>
										<?php endif; ?>
									</div><!-- closes col-md-8 -->
								</div><!-- closes form-group -->

								<div class="form-group button">
									  <button name="submit" type="submit" class="btn btn-primary btn-lg" value="Send Message">Send Message <span class="glyphicon glyphicon-send"></span></button>
								</div><!-- closes form-group -->

							</form>
						</div><!-- closes well -->
						
					</div><!-- closes col-md-6 -->
				</div><!-- closes div -->
			</div><!-- closes div -->
		</header>
		
		<footer>
		
		</footer>
		
		<!-- load JS -->
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.2/jquery.min.js"></script>
        <script src="assets/js/vendor/bootstrap.min.js"></script>
        <script src="assets/js/vendor/modernizr-2.8.3.min.js"></script>
	</body>
</html>
