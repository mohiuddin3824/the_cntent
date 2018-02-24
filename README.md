# the_cntent

The wordPress the_content() shows the whole content of a post. If you want to show custom charecters of a post the click read more button for whole post you should use this code

//Read more function

	function read_more($postless){
		$post_content = explode (" ", get_the_content() );
		
		$less_content = array_slice ($post_content, 0, $postless);
		
		echo implode (" ", $less_content);
	}


Use read_more() function any where and must include any digit on parenthesis as like read_more(20);
