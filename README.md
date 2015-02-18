# jquery.mailchimp
JQuery plugin for mailchimp subscribe form based on original mailchimp code.

# Dependencies

1. [jQuery](http://jquery.com/)
2. [jQuery.form](http://malsup.com/jquery/form/)
3. [jQuery.validate](http://jqueryvalidation.org/)

# Setup

	<script src="/js/jquery-1.11.1.min.js"></script>
	<script src="/js/jquery.form.min.js"></script>
	<script src="/js/jquery.validate.min.js"></script>
	<script src="/js/mailchimp-setup.js"></script>
	<script src="/js/jquery.mailchimp.js"></script>

Content of mailchimp-setup.js depends on your signup form and may be copied from code of mailchimp embedded form.

# Use
	$('form').mailchimpForm()
	$('form.mc-embedded-subscribe-form').each( function () { $(this).mailchimpForm() } )

Yes, works only on one element.

# Changes from original code

1. Localized ( only russian ) server messages, not only jquery validator strings.
2. Still works if you have more than one embedded form on page.
3. Dependencies removed from code, no need to load another one jQuery instance.
