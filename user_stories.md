[x] User Story #1: My product landing page should have a header element with a corresponding id="header".

[x] User Story #2: I can see an image within the header element with a corresponding id="header-img". A company logo would make a good image here.

[x] User Story #3: Within the #header element I can see a nav element with a corresponding id="nav-bar".

[x] User Story #4: I can see at least three clickable elements inside the nav element, each with the class nav-link.

[] User Story #5: When I click a .nav-link button in the nav element, I am taken to the corresponding section of the landing page.

[x] User Story #6: I can watch an embedded product video with id="video".

[x] User Story #7: My landing page has a form element with a corresponding id="form".

[x] User Story #8: Within the form, there is an input field with id="email" where I can enter an email address.

[x] User Story #9: The #email input field should have placeholder text to let the user know what the field is for.

[/] User Story #10: The #email input field uses HTML5 validation to confirm that the entered text is an email address.

    https://devdocs.io/html/element/input/email#Validation suggests that that happens automatically?? Check this

    Currently accepts foo@boo as valid, and redirects to the fCC page. Oops.

    Ha! According to this page, 
        … `a@b` is a valid email address according to the default provided constraints. This is because the email input type allows intranet email addresses by default. To implement different validation behavior, you can use the `pattern` attribute…
    https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types

    I modified the pattern they gave so m@m isn't a valid email address -- but `f@b.m` is, as is /f/@rhul.ac.uk` is :D Not sure if I should try to modify it more? My pattern as it stands is:
    ^[a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*$

    Neither the MDN regex nor mine work, so I seem to be doing something wrong. Will try with just the built-in HTML5 validation and see if it passes the test…

[x] User Story #11: Within the form, there is a submit input with a corresponding id="submit".

[/] User Story #12: When I click the #submit element, the email is submitted to a static page (use this mock URL: https://www.freecodecamp.com/email-submit).

    Do I have to include ```formmethod``` ? Should I send it from the form element using ```action``` instead?

    Cheated and looked at the example. Don't know what theirs does, because CodePen won't allow it to be submitted, but they just have an action, no method. I'll do that. Carry on!

---

[x] User Story #13: The navbar should always be at the top of the viewport.

[x] User Story #14: My product landing page should have at least one media query.

[x] User Story #15: My product landing page should utilize CSS flexbox at least once.
