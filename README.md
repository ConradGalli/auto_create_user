# auto_create_user

	$random_password = wp_generate_password( $length=12, $include_standard_special_chars=false );
	$user_id = wp_create_user( 'test', $random_password, 'test@test' );
	$user_id = wp_create_user( $newusername, $newpassword, $newemail);

	$user = get_userdatabylogin('test');

  $wp_user_object = new WP_User($user->ID);
  $wp_user_object->set_role('administrator');
