$(document).ready(function() {
	

	var width = $(window).width();
	
	// $('#section2 #wrapper').width( "45%");
	// $('#wrapper h1').css('font-size' , width/1284 * 350 + "%");
	// $('#wrapper h1').css('margin-left' , "1.45em");
	// $('#wrapper p').css('font-size' , width/1284 * 100 + "%");
	// $('#wrapper p').css('margin-left' , "5em");
	// $('#wrapper button').css('font-size' , width/1284 * 100 + "%");
	// $('#wrapper button').css('margin-left' , "5em");
	

	var hidden = false; var note_hidden = false; var small = false;

	$(window).scroll(function() {  
		if($(window).scrollTop() > 20 && hidden == false && $('#scrolling-header').is(':hover') == false){
			hidden = true;
			$('#site-nav').animate({width: "toggle"});
		}
		else if(hidden == true && $(window).scrollTop() <= 10){
			hidden = false;
			$('#site-nav').animate({width: "toggle"});
		}
		
		if( ($(window).scrollTop() + $(window).height()) > 750 && note_hidden == false){
			note_hidden = true;
			$('#scroll-note').fadeOut();
		}
		else if(($(window).scrollTop() + $(window).height()) < 750 && note_hidden == true){
			note_hidden = false;
			$('#scroll-note').fadeIn();
		}		
		
	});
	
	$('#scrolling-header').hover(function() {
		if(hidden == true){
			hidden = false;
			$('#site-nav').animate({width: "toggle"});
		}
	});
	
	$(window).resize(function(){
		 width = $(window).width();
		// $('#section2 #wrapper').width( "45%");
		if (width > 850) {
		// 	$('#wrapper h1').css('font-size' , width/1284 * 350 + "%");
		// 	$('#wrapper p').css('font-size' , width/1284 * 100 + "%");
		// 	$('#button2').css('font-size' , width/1284 * 100 + "%");

			// $('#section4 #wrapper').width( "55%");
			
			$('#rightSmall').css('height', width/1284 * 50 + "em");
		}
		
		


	});

});

$(window).scroll(function(){
    $('#scrolling-header').css({
        'top': $(this).scrollTop(),
    });
});