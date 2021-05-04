<template>
    <div id="header">
    <div class="res-menu">
        <div class="wrapper">
            <div class="company-logo"><img src="@/assets/img/sub-head-logo.jpg" alt="Company Logo"/></div>
            <div class="res-els">
                <div class="donation-btn"><a href="#">Donation</a></div>
                <div class="toggle-btn"><i class="fas fa-bars"></i></div>
            </div>
            <div class="cl"><!-- --></div>
        </div>
    </div>
    <div class="main-menu-shell">
        <div class="sub-head">
            <div class="wrapper">
                    <div class="company-logo"><img src="@/assets/img/sub-head-logo.jpg" alt="Company Logo"/></div>
                    <div class="sub-menu">
                        <ul>
                            <li><a href="#">Bliv friviling</a></li>
                            <li><a href="#">Bliv medlem</a></li>
                            <li><a href="#">FAQ</a></li>
                            <li><a href="#">Presse</a></li>
                            <li><a href="#">Visksomheder</a></li>
                        </ul>
                    </div>
                </div>
        </div>
        <div class="main-head">
            <div class="wrapper">
                    <div class="main-menu">
                            <ul>
                                <li><a href="#">Forsiden</a></li>
                                <li><a href="#">Hospice guide</a></li>
                                <li><a href="#">Om os</a></li>
                                <li><a href="#">Nyheder</a></li>
                                <li><a href="#">Søg plads på et hospice</a></li>
                            </ul>
                    </div>
                    <div class="donation-btn"><a href="#">Donation</a></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    

    import jQuery from 'jquery';
    let $ = jQuery;

export default {
    
 mounted: function () {

        $(".toggle-btn").click(function() {
	    $(".main-menu-shell").toggleClass("active");
	});	
    
    },   
 
};
</script>