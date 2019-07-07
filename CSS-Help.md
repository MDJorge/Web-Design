In this wiki, you'll find most of the stuff you need for your subreddit.

Feel free to make a post if you would like further help.

Feel free to add on and improve! (Your account must be at least 100 days old and have 10 karma in the subreddit). 

Album to almost every single snippet from down there: http://imgur.com/a/549RO

Credits to /u/gavin19, /u/sabvegas, and /u/amarsprabhu.

#
># **Table Of Contents**
>Tip: It may be easier to navigate through the album, although not everything is listed there: http://imgur.com/a/549RO

#
># **Tips**
>
>* You cannot link to images on other sites. When the you see code like: `url(%%image%%)` in the snippets code, that doesn't mean you can link to image, you need to upload it and it will give you a replacement for it as shown here: http://i.imgur.com/dLkoy98h.png
>
>* To view the stylesheet of any subreddit, go to the URL:    http://reddit.com/r/subreddit/about/stylesheet just change subreddit to the name of the subreddit you want to look at
>
>* You do not change your reddit logo (in the top left- the alien dude) through CSS. You edit it on the "Community Setting's page located at http://reddit.com/r/subreddit/about/edit . At the bottom of the page you will see the upload form.
>
>* You **cannot** separate snippets with punctuation marks like hyphens, commas, full stops etc. You have to use `/*(whatever)*/`. Don't include the brackets. In fact, just use `/*` in the beginning, and `*/` in the end.
>
>* Gifs are not compatible with CSS
>
>* Older versions of your stylesheets are stored here: 
>http://www.reddit.com/r/subreddit/wiki/revisions/config/stylesheet
>
>* To copy all of another subreddit use my srutils tutorial instead: http://www.reddit.com/r/csshelp/wiki/xyz#wiki_srutils
>
>* To make image flairs use this tutorial instead: http://www.reddit.com/r/csshelp/wiki/xyz#wiki_flair_tutorial or use the link on the sidebar: http://www.reddit.com/r/csshelp/comments/m59kf/  
>
>* Some premade stylesheets for everyone are listed here: http://www.reddit.com/r/csshelp/wiki/themes or alternitavely here: http://www.reddit.com/r/csshelp/wiki/xyz#wiki_shareable_stylesheets
>
>* If you would like some emoticons and such for your subreddit look at the following posts: 
>
>1. Smiley instructions- http://www.reddit.com/r/csshelp/wiki/xyz#wiki_smiley_codes
>
>1. CJ Smiley tutorial- http://www.reddit.com/r/csshelp/wiki/xyz#wiki_cj_smileys
>
>1. f7u12 instructions/tutorial- http://www.reddit.com/r/csshelp/wiki/xyz#wiki_f7u12_rage_faces
>

#
>#Important Note
>
> IF YOUR IMAGES DO NOT SHOW UP, TRY RESIZING THEM: http://www.picresize.com/


#
>#Color Tips
>Any code that look like this is used to specify colors:
>
>     #008000
>
>They are interchangeable with colors names like this as well:
>
>     green
>
>A nice resource for finding hex color codes (the ones that begin with a `#`) is here: http://color.hailpixel.com/ and when you find one that you like just change my colors code(s) with the ones you like
>
>If you would rather use color names use this website instead: http://www.computerhope.com/htmcolor.htm This website lists both the codes and names
>
>If you just want a clear background that will be see through, just insert:
>
>     transparent
>
>As a replacement to the color
>
>Or rgba allows you to use a transparent background

#
>#Stylesheet Tips
>
>##Make a nicer stylesheet:
>
>     .stylesheet-customize-container {
>         width: 100%;
>     }
>     #subreddit_stylesheet {
>         display: block;
>         overflow: hidden;
>     }
>     .sheets {
>         margin: 0;
>     }
>     #stylesheet_contents{
>         font-family: Calibri, Candara, Segoe, "Segoe UI", Optima, Arial, sans-serif;
>         padding: 5px;
>         background-color: #222;
>         color: #ace;
>         border: 2px solid #222;
>         height: 500px;
>         font-size: 13px;
>     }
>     .res-nightmode #stylesheet_contents{
>         background-color: #111;
>         border-color: #111;
>     }
>
>###Preview
>
> http://i.imgur.com/zRPmmH2h.png
>
>##Alternative stylesheet tweek
>
>     .stylesheet-customize-container { width: 100%; }
>     #subreddit_stylesheet { display: block; overflow: hidden; }
>     .sheets { margin: 0;}
>     #stylesheet_contents {
>       padding-left: 5px;
>       padding-top: 5px;
>       background-color: white;
>       color: #042eae;
>       height: 500px;
>     }
>
>###Preview
>
> http://i.imgur.com/fZ0GTB5h.png
>
>##Extremely helpful tip
>
>This thing is movable: http://i.imgur.com/SlB31K9h.png
>

#
>#Flair mini-lesson
> 
> When you assign flair you'll notice a 'css class' box. You can make use of this to easily assign various colour schemes. For example, enter
> 
>     blackwhite
> 
> into the 'css class' box and click save. Then navigate to your stylesheet page
> 
>     www.reddit.com/r/yoursub/about/stylesheet
> 
> and paste in
> 
>     .flair-blackwhite { background-color: #000; color: #fff; }
> 
> Again, click save. If you refresh the page your flair should have a black background and white text. Multiple class names are allowed too (separated by a space) to make combinations possible.
> 
> Instead of the first example you could have used this in the 'css class' box
> 
>     blackbg whitetext
> 
> and this in the stylesheet
> 
>     .flair-whitetext { color: #fff; }
>     .flair-blackbg { background-color: #000; }
>
>##Preview
>
> http://i.imgur.com/n0HaxV1.png
> 
> You just have to ensure that whatever names you enter for the CSS class are prefaced by `.flair-` in the stylesheet. So a class name of purple will become `.flair-purple`.
> 
> credit: [gavin19](http://reddit.com/user/gavin19)
> 
> [Example image](http://i.imgur.com/mPzsnsxh.png)

#
>#Use "multiple stylesheets"
>
>This technique takes advantage of language subdomains, and adds different styles to them.
>
>They basically work the same as normal stylesheets, if you want a dark theme for instance.
>
>     #header { background-color: grey;}
>
>But we only want it in an alternate theme, so that becomes:
>
>     #header:lang(dd) { background-color: grey;}
>
>or
>
>     #header:lang(xx) { background-color: grey;}
>
>but that depends on what you want the URL prefix to be.
>
>`:lang(dd)` changes it at http://dd.reddit.com/r/subreddit
>
>and `:lang(xx)` changes it at http://xx.reddit.com/r/subreddit
>
>Just do that to each property you want to change.
>
>Lets say you want a gray background, normally it would be `body { background-color: gray;}`
>
>To make it alternate, it would be `body:lang(xx) { background-color: gray;}`
>
>Now every-time you visit http://www.xx.reddit.com/r/subreddit It will have a dark background
>
>and continue doing that for each thing you want to change on the alternate stylesheet, just append `:lang(ab)` to your selectors, keep in mind you can only use the following ones in the parentheses:
>
>     en, GB, CA, US, AU, as, dd, cp, tk, zz, yz, xz, yy, or, rd, gr, bl
>
>So `:lang(en)`, `:lang(GB)`, `:lang(CA)`, `:lang(US)`, `:lang(AU)`, `:lang(as)`, `:lang(dd)`, `:lang(cp)`, `:lang(tk)`, `:lang(zz)`, `:lang(yz)`, `:lang(xz)`, `:lang(yy)`, `:lang(or)`, `:lang(rd)`, `:lang(gr)`, `:lang(bl)`
>
>
>You can probable use others, but some are already in use for other languages

#
>#1. Changing the arrows
>
>
>###Preview
>
> http://i.imgur.com/H7sC48w.png
>
>###Code
>
>     /*Arrows*/ 
>     .thing .arrow {
>         height: 25px;
>         width: 25px;
>     }
>     .arrow.up {
>         background: url(%%UpUnclicked%%); 
>     }
>
>     .arrow.upmod { 
>         background: url(%%UpClicked%%); 
>     }
>
>     .arrow.down {
>         background: url(%%DownUnclicked%%); 
>     }
>
>     .arrow.downmod { 
>         background: url(%%DownClicked%%); 
>     }
>
>     /*This allows arrows wider than 15px just change it to the width of your arrows*/
>     .midcol  { min-width:25px !important; }
>
>## Note
> Remember to change to change the height and width values according to the sizes of the images you uploaded

#
>#2. Simple announcement message
> 
>
>###Preview
>
> http://i.imgur.com/tHjgPyW.png
>
>###Code
>    
>     .side .md h4:nth-of-type(1) {
>         list-style-type:none!important;
>         position: absolute;
>         font-size: 14px;
>         display: block;
>         top: 70px; /*Change this in relation to your header's height*/
>         left: 5px; /*adjust this is well*/
>         margin:0;
>         background-color: #f6f7f8!important; /*Change for different background color*/
>         color: #555; /*Change for different for color*/
>         text-align: left;
>         border-radius: 2px;
>         border: 1px solid #dbdbdb;
>         width: auto;
>         padding: 7px 10px 7px 10px;
>         white-space: nowrap;
>         overflow: hidden;
>     }
>     
>     .side .md h1:nth-of-type(1) a {
>         color: rgb(51, 102, 153); /*Changes the colors of the links*/
>     }
>     
>     .content {
>         margin-top:45px; /*Increase or decrease depending on how much room you need*/
>     }
>		
>###Then
>
> you use this sticky by adding a code like so into the sidebar: 
>     `####This is an announcement`


#
>#3. Change name of subscribers/users here now
>
>
>###Preview
>
> http://i.imgur.com/H32PLzo.png
>
>###Code
>
>       /*Changes the name of your subscribers/users here now*/
>       .titlebox .word { display: none }
>       .titlebox .number:after { content: " Users"; }
>       .titlebox .users-online span.number:after { content: " Users here now"; }
>	


#
>#4. Change moderator on side
>
>###Preview
>
> http://i.imgur.com/mRRQqGl.png
>
>###Code
>     
>     /*Changing the word moderators on top of the list of moderators box*/  
>     
>     .sidecontentbox .helplink + .title h1 { font-size: 0}
>     
>     .sidecontentbox .helplink + .title h1:before { font-size: small; content: "Something Else" }	
>	


#
>#5. No more downvotes
>
>##Both posts and comments
>
>###Preview
>
> http://i.imgur.com/JkgGyQn.png
>
>###Code
>
>     .down { display: none; }
>     
>##Posts only
>
>
>###Preview
>
> http://i.imgur.com/v939DSY.png
>
>###Code
>
>     .link .down { display: none; }
>
>##Comments only
>
>
>###Preview
>
> http://i.imgur.com/9WHBIMK.png
>
>###Code
>
>     .comment .down { display: none; }


#
>#6. Simple background image
>
>
>###Preview
>
> http://i.imgur.com/NK1T4m6h.png
>
>###Code
>     
>     /*Simple Background*/
>     body {
>         background: url(%%IMG%%) no-repeat fixed center;
>     }	
>	


#
>#7. Change mail icons
>
>
>###Preview
>
> http://i.imgur.com/3of2mUT.png
>
>###Code
>     
>      /*How to change your mail icons*/
>     #mail {
>         position: relative;
>         display: inline-block;
>         text-indent: -9999px;
>         overflow: hidden;
>         width: 15px; /*These values for the standard mail icon, customize to your own*/
>         height: 10px;
>     }
>     
>     #mail.havemail {
>         background:url(%%MAIL%%);
>     }
>     
>     #mail.nohavemail {
>         background:url(%%NOMAIL%%);
>     }


#    
>#8. In the sidebar, hide the name of the subreddit creator and center the age of the subreddit
>
>
>###Preview
>
> http://i.imgur.com/CSao5E7.png
>
>###Code
>     
>     .titlebox .bottom { font-size: 0; text-align: center; }
>     .bottom .age { float: none; font-size: x-small; }	
>
> If you don't want to center the age of the subreddit then all you need is
>
>     .titlebox .bottom { font-size: 0; }
>     .bottom .age { font-size: x-small; }


#
>#9. Adds an image to the top of the sidebar
>
>
>###Preview
>
> http://i.imgur.com/HQ1MYis.png
>
>###Code
>     
>     /*Add Image to Sidebar*/
>     div.side div.spacer:nth-of-type(1){
>         padding-top: 300px; /*Change "300px" to the height to the height of your image*/
>         background:url(%%Test%%) top center no-repeat;
>     }
>     /*Optional- adds a caption under that image*/
>     div.side div.spacer:nth-of-type(1):before{
>         display:block;
>         margin-top: 10px;
>         width: 300px;
>         content: "This is a caption, edit me to add your own caption.";
>         padding: 0 0 10px;
>         text-align: center; /*delete this line if you no longer want the text centered*/
>         font-family: Georgia, serif; /*Delete this line if you like the normal font better*/
>         font-size: small; /*Change the font-size to your liking*/
>     }	
>	
>##Note
>
> if this one doesn't work, try this one instead: http://www.reddit.com/r/csshelp/wiki/moresnippets#wiki_22._alternative_side_image


#
>#10. Changes the color of self posts based off keywords
>
>
>###Preview
>
> http://i.imgur.com/M9cdg18.png
>
>###Code
>     
>     /*Change color of self posts depending on their title*/
>     #siteTable a[href*="pic"].title { color: #FF6600;} /*This one changes posts that say "pic" to orange*/
>     #siteTable a[href*="find"].title { color: #FF6600;} /*Just change "pic to whatever you want it to change, it just has to be all lowercase. Feel free to change the color*/

#
>#11. Link flairs
>
>
>###Preview
>
> http://i.imgur.com/A0MqsMxh.png
>
>###Code
>     
>     /*Colorful Link Flairs*/
>     /*This adds a colorful little tag to posts*/
>     /*Flairs*/
>     .linkflairlabel { max-width: none; }
>     .linkflair-green .linkflairlabel {color:green}
>     .linkflair-red .linkflairlabel {color:red}
>     .linkflair-blue .linkflairlabel {color:blue}
>     .linkflair-navy .linkflairlabel {color:navy}
>     .linkflair-pink .linkflairlabel {color:pink}
>     .linkflair-orange .linkflairlabel {color:orange}
>     .linkflair-brown .linkflairlabel {color:brown}
>     .linkflair-yellow .linkflairlabel {color:yellow}
>     .linkflair-purple .linkflairlabel {color:purple}
>     .linkflair-black .linkflairlabel {color:black}
>     .linkflair-cyan .linkflairlabel {color:cyan}	
>	
>You now have to click the edit flair link on the sidebar, and once you're there pick a position for them . After that go to "Link Flair Templates" and fill it in like so: http://i.imgur.com/GbLWhsL.png They won't look exactly like those examples though. If you want users to choose their own text just have the little box checked, if not just leave it unchecked.
>


#
>#12. User flairs
>
>
>###Preview
>
> http://i.imgur.com/LRlSR0U.jpg
>
>###Code
>     
>     /*Colorful User Flairs*/
>     .flair{max-width:none; font-weight: 900;}
>     .flair-green{ color:green}
>     .flair-red{ color:red}
>     .flair-orange{ color:orange}
>     .flair-yellow{ color: yellow}
>     .flair-purple{ color:purple }
>     .flair-navy{ color:navy}
>     .flair-black{ color:black}
>     .flair-pink{ color:pink}
>     .flair-cyan{ color:cyan}
>     .flair-brown{ color:brown}
>     .flair-blue{ color:blue}
>And now instead of putting it into the link flair templates put these into the user flair templates, just make sure the little check marks next to each ones are clicked if you want people to be able to choose their own text. http://i.imgur.com/YkoW2zG.jpg
>
> For highly customized user flairs, visit [this](https://www.reddit.com/r/csshelp/wiki/userflair) wiki.

#
>#13. Change color of NSFW
>
>
>###Preview
>
> http://i.imgur.com/H8B5lLB.png
>
>###Code
>     
>     /*Change color of NSFW tag*/
>     .nsfw-stamp acronym {color: purple; border: 1px solid purple; background-color: navy;}
>     /*The first color controls the text color of it, the second color is the outline, and the third one is the background*/


#
>#14. Side by side submit buttons
>
>
>###Preview
>
> http://i.imgur.com/4uGzRsu.png
>
>###Code
>     
>     /*Make submit buttons like /r/whatsinthisthing*/
>     /*Adjust the following to how much room you need for them*/
>     .side {
>         margin-top: 140px; /*This is more than needed*/
>     }
>     
>     .sidebox.submit { 
>         position: absolute; 
>         width: 149px; 
>         top: 140px; /*Change this to position it*/
>     }
>     .sidebox.submit.submit-link { right: auto; }
>     .sidebox.submit.submit-text { left: auto; right: 0; padding-right: 5px; }
>     .side .submit-text { right: 10px;}
>     
>     .submit .morelink { 
>         width: 149px;
>         height: 45px; 
>         border: 0;
>         background: blue; /*Change to whatever color you like*/
>     }
>     
>     .morelink a {
>         display: block;
>         text-align: left; 
>         padding: 3px;
>         color: #fff;
>         font-weight: normal;
>         padding-right: 49px;
>         width: 97px;
>         font-size: 14px;
>         line-height: 20px;
>         border-radius: 0;
>         text-transform: capitalize;
>     }
>     .submit .morelink:hover{  background:#0af;}
>     
>     /* Kills the community button/nub/spacer */
>       .sidebox.create .morelink {display: none;}
>       .sidebox.submit .spacer a, .sidebox.create .spacer a {display: none; }
>       .morelink .nub, .morelink .nub:hover { display: none }
>     

#
>#15. Change the image next to all self posts
>
>
>###Preview
>
> http://i.imgur.com/qjhqIE0.png
>
>###Code
>
>
>     /*Self-post Thumbnail Icon*/
>     .thumbnail.self {
>         height: 50px; /*Adjust to your Images height*/
>         background: url(%%self%%);
>     }	
>     	

#
>#16. Banner image/ header background image
>
>
>###Preview
>
> http://i.imgur.com/ut2J0CZh.png
>
>###Code
>
>     /*Banner*/
>     #header {
>         background: url(%%Banner%%) 0 19px;
>         height: 200px;
>     }
>     #header-bottom-left {
>         position: absolute;
>         bottom: 0;
>     }
>
> Where *Banner* is the name of your uploaded image.

#
>#17. Change subreddit name's color
>
>
>###Preview
>
> http://i.imgur.com/EBkhbJCh.png
>
>####Note
>
>This one changes the color of both the name in the sidebar and the one at the top
>
>###Code
>     
>     /*Your subreddit's name*/
>     .redditname a {
>         color: #fff; /*Change to make your subreddit name a different color*/
>         font-size: 25px; /*Font size of it*/
>     }
>     .redditname a:hover {
>         color: #fff; /*Choose the color for it when hovering over it*/
>         text-decoration:none;
>     }
>	
>
>####Note
>
>This one changes the color of only the one at the top
>
>###Code
>     
>     /*Your subreddit's name*/
>     .pagename a {
>         color: #fff; /*Change to make your subreddit name a different color*/
>         font-size: 25px; /*Font size of it*/
>     }
>     .pagename a:hover {
>         color: #fff; /*Choose the color for it when hovering over it*/
>         text-decoration:none;
>     }
>
>
>####Note
>
>This one changes the color of only the one in the sidebar 
>
>###Code
>     
>     /*Your subreddit's name*/
>      .titlebox h1 a {
>          color: #fff; /*Change to make your subreddit name a different color*/
>          font-size: 25px; /*Font size of it*/
>     }
>     .titlebox h1 a {
>         color: #fff; /*Choose the color for it when hovering over it*/
>         text-decoration:none;
>     }

#
>#18. Rainbow usernames
>
>
>###Preview
>
> http://i.imgur.com/nRq3DQ7.png
>
>###Code
>     
>     /*Makes all usernames rainbow, because why not*/
>     /*Rainbow*/
>     a.author, .res a.author {
>         color: fff!important;
>         background: -moz-linear-gradient(90deg, red, orange, yellow, green, blue, indigo, violet);
>         background: -webkit-linear-gradient(left, red, orange, yellow, green, blue, indigo, violet);
>         background: linear-gradient(to right, red, orange, yellow, green, blue, indigo, violet);
>     }
>	


#
>#19. Rainbows when distinguishing a mod comment/post
>
>
>###Preview
>
> http://i.imgur.com/tNFQRAU.png
>
>###Code
>
>    	/*Make rainbows everytime a mod distinguishes a comment*/
>     a.author.moderator, .res a.author.moderator {
>         color:white!important;
>         background: -moz-linear-gradient(90deg, red, orange, yellow, green, blue, indigo, violet);
>         background: -webkit-linear-gradient(left, red, orange, yellow, green, blue, indigo, violet);
>         background: linear-gradient(to right, red, orange, yellow, green, blue, indigo, violet);
>     }
>	


#
>#20. Change text inside NSFW tag
>
>
>###Preview
>
> http://i.imgur.com/vaTrChp.png
>
>###Code
>
>     /*Change the text in the NSFW tag*/
>     .nsfw-stamp acronym { display: none; }
>     .nsfw-stamp:after {
>         content: 'SPOILER'; /*Change SPOILER to whatever you want it to say*/
>         border: 1px solid;
>         color: #ac3939;
>         padding: 0 2px;
>         border-radius: 3px;
>     }	


#
>#21. Colors
>
>
>###Preview
>
> http://i.imgur.com/puPiEr8h.png
>
>###Code
>
> Visit the "color tips" section above for references
>
>##Header
>
>     #header {background-color: white;}
>
>##Submit buttons
>
>
>###Preview
>
> http://i.imgur.com/hKE7A9u.png
>
>###Code
>
>     .morelink a {
>         color: white;
>         background-color: #449EF8;
>     }
>     .nub { display: none;}
>
>####Note
>
> some really nice submit buttons are linked here: http://www.reddit.com/r/csshelp/wiki/moresnippets#wiki_42._pretty_submit_buttons
>
>##Sidebar
>
>
>###Preview
>
> http://i.imgur.com/erlYkcL.png
>
>###Code
>
>     .side { background-color: white; color: black;}
>     .sidebox .nub {background-color: white;}
>
>##Body
>
>
>###Preview
>
> http://i.imgur.com/qlzULiJh.png
>
>###Code
>
>     body { background-color: white;}
>
>##URL's
>
>
>###Preview
>
> http://i.imgur.com/5mWisFZ.png
>
>###Code
>
>     a { color: orange;}
>     a:hover { text-decoration: underline;}
>
>##Username colors
>
>
>###Preview
>
> http://i.imgur.com/b7xMnBK.png
>
>###Code
>
>     a.author, .res a.author {
>         color:white!important;
>         background-color: green !important;
>     }
>
>##Moderator Distinguish Highlight
>
>
>###Preview
>
> http://i.imgur.com/iGcdiO0.png
>
>###Code
>
>     a.author.moderator, .res a.author.moderator {
>         color:white!important;
>         background-color: green !important;
>     }
>
>##All posts   
>
>###Code
>     
>     #siteTable .title {
>         color: #0f326a;
>     }
>     #siteTable.title:visited,
>     #siteTable a.title:active {
>         color: #142E57;
>     }
>
>##Tabmenu
>
>###Code
>
>     #header .tabmenu li a{
>         color: red;
>         background-color: green;
>         border: 1px solid purple;
>     }
>     #header .tabmenu .selected a{
>         color: white;
>         background-color: red;
>         border: 1px solid green;
>     }
>
>##Comments
>
>###Code
>     
>    .sitetable .comment,
>    .sitetable .comment .comment,
>    .sitetable .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment,
>    .sitetable .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment .comment {
>         background: transparent!important;
>    }
>

#
>#22. Alternative side image 
>
>
>###Preview
>
> http://i.imgur.com/3InILEW.png
>
>###Code
>
>     .side { padding-top: 300px; background: url(%%sideimage%%) no-repeat 0 5px; } /*edit "300px" after padding-top to the height of your image*/
>

#
>#23. Simpler announcement message
>
>
>###Preview
>
> http://i.imgur.com/cIT9xcq.png
>
>###Code
>
>     .titlebox .usertext-body .md ol {
>         list-style: none;
>         position: absolute;
>         top: 163px; /*Change this in relation to your header's height*/
>         left: 8px;
>         margin:0;
>         background-color: #f6f7f8;
>         color: #555;
>         border-radius: 2px;
>         border: 1px solid #dbdbdb;
>         padding: 7px 10px;
>         white-space: nowrap;
>         overflow: hidden;
>     }
>     .titlebox .usertext-body .md ol li {
>         display: inline;
>     }
>     body > .content {
>         margin-top: 45px; /*Increase this number if you want to create more lines/links*/
>     }
>
>## Now
>
>To create the links, add code like this into your sidebar:
>
>     1. [this is an announcement] (http://google.com)
>     2. You may add as many of these as you like
>     3. Just remember that it will get wider and you'll need to increase the margin-top:
>
>You do not need to include more than one if you don't want. Just add as many as you like, except remember to increase the `margin-top:`
>

#
>#24. Change the color of Subscribe/unsubscribe button
>
> ##Change color of the subscribe button
>
>
>###Preview
>
> http://i.imgur.com/poHuZ5m.png
>
>###Code
>
>     .fancy-toggle-button .add {
>             background: none;
>             background-color: red;
>         }
>
>##Change the color of the unsubscribe button
>
>
>###Preview
>
> http://i.imgur.com/od3ncrA.png
>
>###Code
>
>     .fancy-toggle-button .remove {
>             background: none;
>             background-color: red;
>         }

#
>#25. Remove the "and X more >>" from the sidebar mod list
>
>
>###Preview
>
> http://i.imgur.com/GNuQlOO.png
>
>###Code
>
>     .sidecontentbox .more a {
>         display: none;
>     }

#
>#26. /r/canada hover boxes
>
> By /u/sweet_nightmares
>
>###Preview
>
> http://i.imgur.com/L5nfwwt.png
>
>Hover box preview: http://i.imgur.com/ltbdBrr.gif
>
>###Code
>
>     /***** Sidebar headings *****/
>     .titlebox blockquote {
>         border: 1px solid #AAA;
>         text-shadow: 0 1px 0 white;
>         color: #787878;
>         font-weight: bold;
>         border-radius: 10px;
>     }
>     .titlebox {
>         padding: 10px;
>         background: transparent; /*Sidebar Background color*/
>         border: 1px solid #AAA; /*Sidebar border color*/
>         color: #787878; /*Text color in sidebar*/
>         border-radius: 10px;
>     }
>     /***** Collapsible menu *****/
>     .titlebox .md h3 + ul {
>         margin: 0 2em;
>         padding: 3px;
>      }
>     .titlebox .md h3, div.titlebox .md h3 a {
>         color: #eee; /*General Header text color*/
>      }
>     .titlebox .md h3 + ul {
>         display: none;
>      }
>     .titlebox .md h3:hover + ul,
>     .titlebox .md h3 + ul:hover {
>         display: block;
>     }
>     .titlebox .md h3 + ul li:hover {
>         background-color: #eee; 
>       /*Color you seen when ^ hovering over sidebar items*/
>     }
>     .res-nightmode .titlebox .md h3 + ul li:hover {
>         background-color: #393939;
>       /*Color you seen when ^ hovering over sidebar items- Nightmode*/
>     }
>     .titlebox .md h3 {
>         background-color: #96bf43; /*### background color*/
>         color: #fff; /*### Text color*/
>         width: 280px;
>         line-height: 23px;
>         font-weight: normal;
>         font-size: 16px;
>         cursor: pointer;
>         padding-left: 20px;
>         margin: 4px 0 0 -11px;
>     }
>     .res-nightmode .titlebox .md h3 { 
>         background-color: #7a9642; /*Nightmode background color*/
>     }
>     .titlebox .md h3:after {
>         margin-bottom: 10px;
>     }
>     .titlebox .md h3:before { 
>         content: "+"; 
>         color: #fff; /*color of the + in ###*/
>     padding-right: 5px; 
>     } 
>     .titlebox .md h3 + ul {
>         line-height: 1.7em
>     }
>
>
>This `###Title` is known as a header, just add `#`'s before your text. This CSS targets h3 headers specifically, so you need to use ###, eg
>     
>     ###Title
>     * First item
>     * Second item
>     * Third item
>     * Fourth item
>     * Fifth item
>
>
> The items below that are the list items that are hidden from view until you hover the header. End each line with two spaces and start each list item with an * and a space. 

#
>#27. No downvoting unless subscribed
>
>
>###Preview
>
> http://i.imgur.com/kV8VfCV.png
>
>###Code
>
>     body:not(.subscriber) .down
>     { 
>         visibility: hidden !important;
>     }
>     body:not(.subscriber) #siteTable:before
>     {
>          content: "You are not a member of this community. Please respect that by not downvoting.";
>         display: block;
>         max-width: 800px;
>         background-color: #F6E69F;
>         padding: 5px 10px;
>         margin: 5px 305px 5px 0px;
>         border: 1px solid orange;
>         font-size: small;
>     }
>
>###Note
>
> You can remove the second half of the snippet, to hide the message at the top.

#
>#28. No participation mode
>
>
>###Preview
>
> http://i.imgur.com/lWU48e4h.png
>
>###Code
>
> http://www.reddit.com/r/NoParticipation/wiki/installation

#
>#29. Srutils, Image flairs, themes, and emotes
>
>##Srutils
>
>* To copy all of another subreddit use my srutils tutorial instead: http://www.reddit.com/r/csshelp/wiki/xyz#wiki_srutils
>
>##Image flairs
>
>* To make image flairs use this tutorial instead: http://www.reddit.com/r/csshelp/wiki/xyz#wiki_flair_tutorial or use the link on the sidebar: http://www.reddit.com/r/csshelp/comments/m59kf/
>
>##Themes
>
>* Some premade stylesheets for everyone are listed here: http://www.reddit.com/r/csshelp/wiki/themes or alternitavely here: http://www.reddit.com/r/csshelp/wiki/xyz#wiki_shareable_stylesheets
>
>##Emotes
>
>If you would like some emoticons and such for your subreddit look at the following posts: 
>
>###Smiley instructions- 
>
>http://www.reddit.com/r/csshelp/wiki/xyz#wiki_smiley_codes
>
>###CJ Smiley tutorial- 
>
>http://www.reddit.com/r/csshelp/wiki/xyz#wiki_cj_smileys
>
>###f7u12 rage faces instructions/tutorial- 
>
>http://www.reddit.com/r/csshelp/wiki/xyz#wiki_f7u12_rage_faces

#
>#30. Fix for floating pagename/tabs
>
>
>###Preview
>
> http://i.imgur.com/0dyKw1j.png
>
>###Code
>
>
>     #header-bottom-left {
>         position: absolute;
>         bottom: 0;
>     }

#
>#31. Redirect to a Different Subreddit
>
>###Preview
>
>http://i.imgur.com/oeMdR.png
>
>###Code
>  
> (Change /r/YourSubreddit to your subreddit's name)
> 
> THE SUBREDDIT NAME IN THE CODE AND IN THE SIDEBAR ARE CASE SENSITIVE TO ONE ANOTHER!
> Type this in the sidebar section of community settings:
> 
>     [Click anywhere to continue to /r/YourSubreddit](http://www.reddit.com/r/YourSubreddit)
> 
> Then, type this in the stylesheet:
> 
>     .side a[href*="/r/YourSubreddit"] {
>         position:fixed;
>         top:0; left:0;
>         height:100%;
>         width:100%;
>         z-index:9999;
>         background:#000;
>         color:#FFF;
>         font-size:50px;
>         line-height:500%;
>         text-align:center;
>         }
>     body {
>         overflow: hidden;
>         }
>     .moderator .styleToggle {
>         z-index: 99999;
>         background-color: white;
>         text-align: center;
>         }

#
>#32. Message for Non-Subscribers
>
>
>###Preview
>
> http://i.imgur.com/PmnPAN8.png
>
>###Note
>
> Upload [this image](http://i.imgur.com/koG26.png) entitled "warning"
>
>###Code
>
> 
>     body:not(.subscriber) > .content:before{  
>         content: url(%%warning%%) " You're not subscribed to r/subreddit yet! Click the subscribe button on the right to add the subreddit to your frontpage ";
>     }

#
>#33. Submit warning like /r/photoshopbattles
>
>
>###Preview
>
> http://i.imgur.com/wi2Cyarh.png
>
>###Code
>
>     .sidebox.submit:hover:before{
>         position:fixed;
>         display:block;
>         top:0;
>         text-align:center;
>         background-color:#7da5ce; /*Edit to your liking*/
>         color:white; /*Font color*/
>         z-index:1000;
>         padding:5px 0;
>         width:100%;
>         left:0;
>         font-size:32px;
>         font-weight:normal;
>         content:"Please read the rules before posting."
>     }

#
>#34. Add text to the submit page
>
>
>###Preview
>
> http://i.imgur.com/92tQNxZ.png
>
>###Code
>
>     #link-desc, #text-desc {font-size: 0px;}/*Hides default text*/
>     /* Adds text to the submission page*/
>     #link-desc:after, #text-desc:after {
>         display: block;
>         font-weight: bold; /*Delete this line if you don't want bold text*/
>         color: black; /*You could also change it to something more attention grabbing*/
>         content: "Insert text here";
>         font-size: 12px;
>     } 

#
>#35. Add an image to the sidebar while using /r/boxed's theme
>You have to edit the code rather than pasting new blocks of code on top of it. look in my code for the following code:
>
>
>###Preview
>
> http://i.imgur.com/co51meCh.png
>
>###Code
>
>     .side {
>         width: 300px;
>         margin: 50px 20px 20px 20px;
>         padding: 5px !important;
>         z-index: 0;
>         border: 0;
>         box-shadow: 0px 1px 3px 1px #A5B9CE;
>         overflow: hidden;
>       }
>
>And replace it with
>
>     .side {
>         width: 300px; /*Keep the images width at 300px*/
>         margin: 50px 20px 20px 20px;
>         padding: 300px 5px 5px 5px !important;
>         /*Change 300px in the above line to the height of your image*/
>         background: url(%%EXAMPLE%%) no-repeat;
>         background-color: #FFFFFF;
>         z-index: 0;
>         border: 0;
>         box-shadow: 0px 1px 3px 1px #A5B9CE;
>         overflow: hidden;
>     }

#
>#36. Spoiler tags
> 
>
>###Preview
>
> http://i.imgur.com/TRkYFrI.png
>
>###Code
>
>     a[href$="/spoiler"], a[href$="#spoiler"], a[href$="/s"], a[href$="#s"] {  
>         background: #000 !important;  
>         color: #000 !important  
>     }  
>     a[href$="/spoiler"]:hover, a[href$="#spoiler"]:hover, a[href$="/s"]:hover, a[href$="#s"]:hover {  
>         color: #FFF !important  
>     }  
>
>##How To
>
> Then, to use them insert code like this into comments, the ones with `#` are mobile friendly
>
>     [This is the message](/spoiler)
>     [This is another spoiler](#spoiler)
>     [This code allows for 4 different spoiler codes](/s)
>     [Another spoiler message](#s)

#
>#37. Report button hover message
>
>
>###Preview
>
> http://i.imgur.com/enC2P8H.png
>
>###Code
>
>     .report-button:hover:after {
>         position: absolute;
>         white-space: normal;
>         display: block;
>         z-index: 1000;
>         width: 350px;
>         padding: 5px;
>         border: 0px solid #333;
>         background: #fca;
>         content: "Please also message the moderators a link and reason why you are reporting this, thanks. ";
>         text-align: center;
>         font-size: 10px;
>         color: red;
>         margin-left: 25px;
>         margin-top: 5px;
>         -moz-border-radius: 4px;
>         border-radius: 4px;
>         -webkit-border-radius: 4px
>     }
>
>
>
>
>
> ##Reminder 
>you can change any of the colors you see above using the color tips section of this tutorial

#
>#38. Downvote Hover Warning
>
>
>###Preview
>
> http://i.imgur.com/ItHm6ox.png
>
>###Code
>
>     .arrow.down:hover:before {
>          position: absolute;
>          z-index: 1000;
>          padding: 5px;
>          border: 0;
>          background: #fca;
>          content: "Don't downvote simply because you don't agree";
>          text-align: center;
>          font-size: 10px;
>          color: #f00;
>          margin-left: 25px;
>          margin-top: 5px;
>          border-radius: 4px;
>     }
>
>
>
>
>
> ##Reminder 
>you can change any of the colors you see above using the color tips section of this tutorial

#
>#39. Sidebar image that changes
>
> http://www.reddit.com/r/csshelp/wiki/snippets#wiki_random_image_above_sidebar
>

#
>#40.  Buttons from /r/naut
>
>     /*/r/naut buttons*/
>
>     button,#search input[type="submit"],.wiki-page .wiki-page-content .wiki_button{
>         margin:3px 3px 3px 3px;
>         padding:0px 8px 1px 8px;
>         background-color:#ffffff;
>         border:1px solid #d4d4d4;
>         border-radius:2px;
>         -webkit-box-shadow:0 1px 0 #e2e0e0;
>         box-shadow:0 1px 0 #e2e0e0;
>         color:#737373!important;
>         text-transform:capitalize;
>         font-weight:bold;
>         line-height:26px;
>         cursor:default;
>     }
>     button:hover,#search input[type="submit"]:hover,.wiki-page .wiki-page-content .wiki_button:hover {
>         padding-bottom:0px;
>         border-color:#bababa;
>         border-bottom-width:2px;
>         color:#333!important;
>     }
>     button:active,#search input[type="submit"]:active,.wiki-page .wiki-page-content .wiki_button:active {
>         padding-bottom:0px;
>         background-color:#e5e5e5;
>         border-color:#a7a7a7;
>         border-top-width:2px;
>         border-bottom-width:1px;
>         -webkit-box-shadow:none;
>         box-shadow:none;
>         color:#333!important;
>         line-height:25px;
>     }
>     .res .blueButton {
>         padding:2px 3px!important;
>         background-color:#53a93f!important;
>         border:none!important;
>         border-radius:0px!important;
>     }
>     .RESSubscriptionButton {
>         background-color:white!important;
>         border:0px solid!important;
>         border-radius:0px!important;
>         color:#5b92fa!important;
>     }
>     
>     /* Nightmode buttons*/
>     
>     body.res-nightmode button,body.res-nightmode #search input[type="submit"],body.res-nightmode .wiki-page .wiki-page-content .wiki_button{
>         padding: 0px 8px 0px 8px;
>         background-color: transparent;
>         border: 1px solid #414955;
>         border-radius: 0px;
>         -webkit-box-shadow: none;
>         box-shadow: none;
>         color: #e5e5e5!important;
>         line-height: 28px;
>     }
>     body.res-nightmode button: hover,body.res-nightmode #search input[type="submit"]: hover,body.res-nightmode .wiki-page .wiki-page-content .wiki_button: hover{
>         padding-bottom: 0px;
>         border-color: #414955;
>         border-width: 1px;
>         color: #fff!important;
>         line-height: 28px;
>         background-color: #1C1F26;
>     }
>     body.res-nightmode button: active,body.res-nightmode #search input[type="submit"]: active,body.res-nightmode .wiki-page .wiki-page-content .wiki_button: active{
>         padding-bottom: 0px;
>         background-color: #1C1F26;
>         border-color: #414955;
>         border-width: 1px;
>         -webkit-box-shadow: none;
>         box-shadow: none;
>         color: #fff!important;
>         line-height: 28px;
>     }
>     .RESSubscriptionButton { background-color:transparent!important; }

#
>#41. Linkable sidebar image
>
>     .side { margin: 310px 5px 0; }
>     .side a[href="http://www.yourlink.com"] {
>         position: absolute;
>         top: 126px; /*distance from the top*/
>         height:300px; /*adjust to the height of your image*/
>         width:300px; /*always try and keep this at 300px*/
>         background:url(%%sideimage%%) no-repeat 0 0;
>     }
>
>Change the URL I used in the code above to the link you want, also in your sidebar add:
>
>     [](http://www.yourlink.com)
>
>The links are case sensitive, so make sure the code and sidebar links are the same. 

#
>#42. Pretty Submit buttons
>
>Submit Button Preview:
>
>http://i.imgur.com/EvO04fW.png
>
>##Version 1
>
>
>###Preview
>
> http://i.imgur.com/k5PsJNK.png
>
>###Code
>
>     /* PRETTY SUBMIT LINKS by /u/RainbowCrash*/
>     .morelink
>     {
>         font-weight:normal;
>         letter-spacing:0;
>         background: red;
>         border: none;
>         -moz-border-radius:2px;
>         -webkit-border-radius:2px;
>         -o-border-radius:2px;
>         -ms-border-radius:2px;
>         -khtml-border-radius:2px;
>         border-radius:2px;
>         height: 30px;
>         line-height: 30px;
>         overflow: hidden;
>         color: white;
>     }
>     
>     .morelink:hover
>     {
>         background: #A7B9CB;
>         background-color: #FF0000;
>         border-color: #FF0000;
>     }
>     
>     .morelink .nub 
>     {
>         display: none;
>     }
>     
>     .morelink 
>     {
>         color:#FFF; 
>         font-family:Verdana, Arial, sans-serif; 
>         font-size:16px; 
>         width: 145px;
>     }
>     
>     .morelink a, .morelink a:hover
>     {
>         color: white;
>     }
>     
>     .sidebox.submit-link .morelink::before 
>     {
>         display: block;
>         clear: none;
>         content: "Submit a Link";
>         font-size: 95%;
>     }
>     
>     .sidebox.submit-text .morelink::before 
>     {
>         display: block;
>         clear: none;
>         content: "Submit a Self Post";
>         font-size: 90%;
>     }
>     
>     .sidebox.submit .morelink a 
>     {
>         position: absolute;
>         top: 0;
>         padding-left: 1000px;
>         font-size: 0px;
>         text-align: right;
>         color: #56a6f7;
>     }
>     
>     .sidebox.submit.submit-link {
>         width: 150px;
>     }
>     
>     .sidebox.submit.submit-text
>     {
>         margin-top: -42px; /*Edit this is the buttons aren't parallel*/
>         margin-left: 153px;
>     }
>     
>     .sidebox.create 
>     {
>         display: none;
>     }
>     
>     .sidebox.submit.disabled 
>     {
>         display: none;
>     }
>     /* NIGHTMODE FIXES */
>     .res-nightmode .sidebox.submit.submit-text
>     {
>         background: none !important;
>         margin-top: -45px;
>         margin-left: 153px;
>     }
>     
>     .res-nightmode .sidebox 
>     {
>         padding-left: 0px !important;
>         border: 2px solid #151515 !important;
>     }
>     
>     .res-nightmode .morelink 
>     {
>          height: 29px !important;
>     }
>     
>     .res-nightmode .morelink
>     {
>         background:rgb(39, 63, 87) !important;
>     }
>     
>     .res-nightmode .morelink:hover
>     {
>         background: #449ef8 !important;
>         background-color: #9edbf8 !important;
>         border-color: #9edbf8 !important;
>     }
>     /* END NIGHTMODE FIX */
>     /* END PRETTY SUBMIT LINKS */
>
>
>
>
>## Version 2
>
>
>###Preview
>
> http://i.imgur.com/LtpFlBW.png
>
>###Code
>
>     /* PRETTY SUBMIT LINK (1 bar) by /u/RainbowCrash (modified by Sabvegas)*/
>     /* Remove submit text button */
>     .submit-text { display:none; }
>     /*end remove submit text button*/
>     .morelink
>     {
>         font-weight:normal;
>         letter-spacing:2px;
>         background:  purple ;
>         border: none;
>         -moz-border-radius:2px;
>         -webkit-border-radius:2px;
>         -o-border-radius:2px;
>         -ms-border-radius:2px;
>         -khtml-border-radius:2px;
>         border-radius:2px;
>         height: 30px;
>         line-height: 30px;
>         overflow: hidden;
>         color: white;
>     }
>     .morelink:hover
>     {
>         background: #A7B9CB;
>         background-color: #FF0000;
>         border-color: #FF0000;
>     }
>     
>     .morelink .nub 
>     {
>         display: none;
>     }
>     
>     .morelink 
>     {
>         color:#FFF; 
>         font-family: Calibri, Candara, Segoe, "Segoe UI", Optima, Arial, sans-serif;
>         font-size:19px; 
>         width: 301px;
>     }
>     
>     .morelink a, .morelink a:hover
>     {
>         color: white;
>     }
>     
>     .sidebox.submit-link .morelink::before 
>     {
>         display: block;
>         clear: none;
>         content: "Submit a New Post";
>         font-size: 95%;
>        overflow: hidden;
>     }
>     
>     .sidebox.submit .morelink a 
>     {
>         position: absolute;
>         top: 0;
>         padding-left: 1000px;
>         font-size: 0px;
>         text-align: right;
>         color: #56a6f7;
>     }
>     
>     .sidebox.submit.submit-link {
>         width: 150px;
>     }
>     .sidebox.create 
>     {
>         display: none;
>     }
>     
>     .sidebox.submit.disabled 
>     {
>         display: none;
>     }
>     /* NIGHTMODE FIXES */
>     .res-nightmode .sidebox.submit.submit-text
>     {
>         background: none !important;
>         margin-top: -45px;
>         margin-left: 153px;
>     }
>     
>     .res-nightmode .sidebox 
>     {
>         padding-left: 0px !important;
>         border: 2px solid #151515 !important;
>     }
>     
>     .res-nightmode .morelink 
>     {
>          height: 29px !important;
>     }
>     
>     .res-nightmode .morelink
>     {
>         background:rgb(39, 63, 87) !important;
>     }
>     
>     .res-nightmode .morelink:hover
>     {
>         background: #449ef8 !important;
>         background-color: #9edbf8 !important;
>         border-color: #9edbf8 !important;
>     }
>     /* END NIGHTMODE FIX */
>     /* END PRETTY SUBMIT LINKS */
>
>
>
>
>
>##Version 3
> As seen at /r/mindashq
>
>###Preview
>
> http://i.imgur.com/DBdCeAj.png
>
>###Code
>
>     /* from /r/mindashq */
>     .sidebox.submit {
>     width: 300px;
>     }
>     body:not(.listing-page) .morelink {
>     border-color: #5ba2fd!important;
>     border-radius: 2px!important;
>     background: none transparent;
>     background-color: #acd9fc;
>     background-image: -webkit-linear-gradient(top,#acd9fc,#8ccbfc)!important;
>     background-image: -moz-linear-gradient(top,#acd9fc,#8ccbfc)!important;
>     background-image: linear-gradient(top,#acd9fc,#8ccbfc)!important;
>     color: #2154a3;
>     }
>     body:not(.listing-page) .morelink a {
>     color: #2154a3!important;
>     text-shadow: 1px 1px 2px #eee;
>     }
>     body .morelink {
>     padding: 4px 10px;
>     border-color: #3079ed!important;
>     border-radius: 2px!important;
>     background: none transparent;
>     background-color: #5ba2fd;
>     background-image: -webkit-linear-gradient(top,#5ba2fd,#4b8adb)!important;
>     background-image: -moz-linear-gradient(top,#5ba2fd,#4b8adb)!important;
>     background-image: linear-gradient(top,#5ba2fd,#4b8adb)!important;
>     color: #fff;
>     font-weight: normal;
>     letter-spacing: 0;
>     }
>     body .morelink:hover,
>     body:not(.listing-page) .morelink:hover {
>     border-color: #08c;
>     background: none transparent;
>     background-color: #357ae8;
>     background-image: -webkit-linear-gradient(top,#4d90fe,#357ae8)!important;
>     background-image: -moz-linear-gradient(top,#4d90fe,#357ae8)!important;
>     background-image: linear-gradient(top,#4d90fe,#4787ed)!important;
>     color: #fff;
>     }
>     body .morelink a {
>     color: #fff!important;
>     font-weight: bold;
>     font-size: 16px;
>     text-shadow: 1px 1px 2px #0f0f0f;
>     }
>     body .morelink a:hover,
>     body:not(.listing-page) .morelink:hover a,
>     body:not(.listing-page) .morelink a:hover {
>     color: #fff!important;
>     text-shadow: 1px 1px 2px #0f0f0f!important;
>     }
>     body .morelink .nub,
>     body .morelink:hover .nub,
>     body .disabled .morelink .nub,
>     body .disabled .morelink:hover .nub {
>     background: none transparent!important;
>     }
>     body .disabled .morelink,
>     body .disabled .morelink:hover {
>     border-color: #f5f5f5!important;
>     background-color: #eee;
>     background-image: none!important;
>     }
>     body .disabled .morelink a,
>     body .disabled .morelink a:hover {
>     color: #aaa!important;
>     text-shadow: none!important;
>     cursor: default!important;
>     }
>
>####Optional Extra Code
>
>     .side {
>	     margin: 0 20px;
>	     padding: 0 10px;
>	     width: 300px;
>	     line-height: 1.3;
>	     z-index: 10;
>     }
>
>
>##Version 4
> As seen at /r/mindashq
>
>###Preview
>
> http://i.imgur.com/bwqCCQj.png
>
>###Note
>
> If you want to use this button please navigate to http://reddit.com/r/yoursubreddit/about/edit and input the following: http://i.imgur.com/DiDnrFq.png
>
>###Code
>
>     /* from /r/mindashq */
>     .sidebox.submit {
>     width: 300px;
>     }
>     body:not(.listing-page) .morelink {
>     border-color: #5ba2fd!important;
>     border-radius: 2px!important;
>     background: none transparent;
>     background-color: #acd9fc;
>     background-image: -webkit-linear-gradient(top,#acd9fc,#8ccbfc)!important;
>     background-image: -moz-linear-gradient(top,#acd9fc,#8ccbfc)!important;
>     background-image: linear-gradient(top,#acd9fc,#8ccbfc)!important;
>     color: #2154a3;
>     }
>     body:not(.listing-page) .morelink a {
>     color: #2154a3!important;
>     text-shadow: 1px 1px 2px #eee;
>     }
>     body .morelink {
>     padding: 4px 10px;
>     border-color: #3079ed!important;
>     border-radius: 2px!important;
>     background: none transparent;
>     background-color: #5ba2fd;
>     background-image: -webkit-linear-gradient(top,#5ba2fd,#4b8adb)!important;
>     background-image: -moz-linear-gradient(top,#5ba2fd,#4b8adb)!important;
>     background-image: linear-gradient(top,#5ba2fd,#4b8adb)!important;
>     color: #fff;
>     font-weight: normal;
>     letter-spacing: 0;
>     }
>     body .morelink:hover,
>     body:not(.listing-page) .morelink:hover {
>     border-color: #08c;
>     background: none transparent;
>     background-color: #357ae8;
>     background-image: -webkit-linear-gradient(top,#4d90fe,#357ae8)!important;
>     background-image: -moz-linear-gradient(top,#4d90fe,#357ae8)!important;
>     background-image: linear-gradient(top,#4d90fe,#4787ed)!important;
>     color: #fff;
>     }
>     body .morelink a {
>     color: #fff!important;
>     font-weight: bold;
>     font-size: 16px;
>     text-shadow: 1px 1px 2px #0f0f0f;
>     }
>     body .morelink a:hover,
>     body:not(.listing-page) .morelink:hover a,
>     body:not(.listing-page) .morelink a:hover {
>     color: #fff!important;
>     text-shadow: 1px 1px 2px #0f0f0f!important;
>     }
>     body .morelink .nub,
>     body .morelink:hover .nub,
>     body .disabled .morelink .nub,
>     body .disabled .morelink:hover .nub {
>     background: none transparent!important;
>     }
>     body .disabled .morelink,
>     body .disabled .morelink:hover {
>     border-color: #f5f5f5!important;
>     background-color: #eee;
>     background-image: none!important;
>     }
>     body .disabled .morelink a,
>     body .disabled .morelink a:hover {
>     color: #aaa!important;
>     text-shadow: none!important;
>     cursor: default!important;
>     }
>     .sidebox.submit {
>     width: 147px;
>     word-spacing: 1px;
>     letter-spacing: -1px;
>     }
>     .sidebox.submit-link {
>     display: block;
>     margin-left: 0px;
>     }
>     .sidebox.submit-link .morelink .nub:before {
>     content: 'OR';
>     position: relative;
>     top: 4px;
>     margin-left: 12px;
>     padding: 5px;
>     height: auto;
>     border: 1px solid #fbfbf9;
>     border-radius: 20px;
>     background-color: #fbfbf9!important;
>     color: #2977c6;
>     font-weight: bold;
>     font-size: 12px;
>     text-shadow: 1px 1px 1px #fff,1px 1px 2px #808088;
>     z-index: 1;
>     }
>     .sidebox.submit-text {
>     margin-left: 152px;
>     text-align: right;
>     }
>     body.res-nightmode .sidebox.submit-link .morelink .nub {
>     display: block!important;
>     }
>     body.res-nightmode .sidebox.submit-link .morelink .nub:before {
>     border: 1px solid #222222;
>     background-color: #222222!important;
>     color: #bb6107;
>     text-shadow: 1px 1px 1px #000,1px 1px 2px #1f1f1f;
>     }
>     .sidebox.submit {
>     position: absolute;
>     top: 105px; /*Tweak this as per the header height*/
>     }
>     .sidecontentbox a.helplink {
>     position: absolute;
>     top: 146px; /*Tweak this as per the header height*/
>     font-size: 12px;
>     }
>     .sidecontentbox a.helplink:before {
>     content: 'Or';
>     margin: 0px .3em 0px 1.5em;
>     color: #808080;
>     }
>     .sidecontentbox a.helplink:after {
>     content: 'for help'; /*Tweak this for message after the link*/
>     margin: 0px 0px 0px .3em;
>     color: #808080;
>     }
>     .side .spacer #search,
>     body.search-page .side .titlebox {
>     margin-top: 70px;
>     }
>     body.submit-page .sidecontentbox a.helplink {
>     top: 115px; /*Tweak this as per the header height*/
>     right: 370px;
>     }
>     body.submit-page .side .spacer #search {
>     margin-top: 0px;
>     }
>     div.side{margin-top:5px;} /*Increase this number to give your buttons more room*/
>
>
>####Optional Extra Code
>
>     .side {
>	     margin: 0 20px;
>	     padding: 0 10px;
>	     width: 300px;
>	     line-height: 1.3;
>	     z-index: 10;
>     }
>
>
>
>##Version 5
> As seen at /r/mindashq
>
>###Preview
>
> http://i.imgur.com/lMGyyJ4.png
>
>###Note
>
> If you want to use this button please navigate to http://reddit.com/r/yoursubreddit/about/edit and input the following: http://i.imgur.com/DiDnrFq.png
>
>###Code
>
>     /* from /r/mindashq */
>     .sidebox.submit {
>     width: 300px;
>     }
>     body:not(.listing-page) .morelink {
>     border-color: #5ba2fd!important;
>     border-radius: 2px!important;
>     background: none transparent;
>     background-color: #acd9fc;
>     background-image: -webkit-linear-gradient(top,#acd9fc,#8ccbfc)!important;
>     background-image: -moz-linear-gradient(top,#acd9fc,#8ccbfc)!important;
>     background-image: linear-gradient(top,#acd9fc,#8ccbfc)!important;
>     color: #2154a3;
>     }
>     body:not(.listing-page) .morelink a {
>     color: #2154a3!important;
>     text-shadow: 1px 1px 2px #eee;
>     }
>     body .morelink {
>     padding: 4px 10px;
>     border-color: #3079ed!important;
>     border-radius: 2px!important;
>     background: none transparent;
>     background-color: #5ba2fd;
>     background-image: -webkit-linear-gradient(top,#5ba2fd,#4b8adb)!important;
>     background-image: -moz-linear-gradient(top,#5ba2fd,#4b8adb)!important;
>     background-image: linear-gradient(top,#5ba2fd,#4b8adb)!important;
>     color: #fff;
>     font-weight: normal;
>     letter-spacing: 0;
>     }
>     body .morelink:hover,
>     body:not(.listing-page) .morelink:hover {
>     border-color: #08c;
>     background: none transparent;
>     background-color: #357ae8;
>     background-image: -webkit-linear-gradient(top,#4d90fe,#357ae8)!important;
>     background-image: -moz-linear-gradient(top,#4d90fe,#357ae8)!important;
>     background-image: linear-gradient(top,#4d90fe,#4787ed)!important;
>     color: #fff;
>     }
>     body .morelink a {
>     color: #fff!important;
>     font-weight: bold;
>     font-size: 16px;
>     text-shadow: 1px 1px 2px #0f0f0f;
>     }
>     body .morelink a:hover,
>     body:not(.listing-page) .morelink:hover a,
>     body:not(.listing-page) .morelink a:hover {
>     color: #fff!important;
>     text-shadow: 1px 1px 2px #0f0f0f!important;
>     }
>     body .morelink .nub,
>     body .morelink:hover .nub,
>     body .disabled .morelink .nub,
>     body .disabled .morelink:hover .nub {
>     background: none transparent!important;
>     }
>     body .disabled .morelink,
>     body .disabled .morelink:hover {
>     border-color: #f5f5f5!important;
>     background-color: #eee;
>     background-image: none!important;
>     }
>     body .disabled .morelink a,
>     body .disabled .morelink a:hover {
>     color: #aaa!important;
>     text-shadow: none!important;
>     cursor: default!important;
>     }
>     .sidebox.submit {
>     width: 147px;
>     word-spacing: 1px;
>     letter-spacing: -1px;
>     }
>     .sidebox.submit-link {
>     position: relative;
>     display: block;
>     margin-left: 0px;
>     text-indent: 0px;
>     }
>     .sidebox.submit-link .morelink .nub:before {
>     content: 'OR';
>     position: relative;
>     top: 4px;
>     margin-left: 12px;
>     padding: 5px;
>     height: auto;
>     border: 1px solid #fbfbf9;
>     border-radius: 20px;
>     background-color: #fbfbf9!important;
>     color: #2977c6;
>     font-weight: bold;
>     font-size: 12px;
>     text-shadow: 1px 1px 1px #fff,1px 1px 2px #808088;
>     z-index: 1;
>     }
>     .sidebox.submit-text {
>     position: relative;
>     float: right;
>     margin-top: -44px; /*If the buttons aren't parallel, adjust this line*/
>     text-align: right;
>     }
>     body.res-nightmode .sidebox.submit-link .morelink .nub {
>     display: block!important;
>     }
>     body.res-nightmode .sidebox.submit-link .morelink .nub:before {
>     border: 1px solid #222222;
>     background-color: #222222!important;
>     color: #bb6107;
>     text-shadow: 1px 1px 1px #000,1px 1px 2px #1f1f1f;
>     }
>     body.res-nightmode .sidebox.submit-text {
>     top: -2px;
>     }
>####Optional Extra Code
>
>     .side {
>	     margin: 0 20px;
>	     padding: 0 10px;
>	     width: 300px;
>	     line-height: 1.3;
>	     z-index: 10;
>     }

#
>#43. Header shadow gradient
>
>###Preview
>
> http://i.imgur.com/nPSYOIu.png
>
>###Code
>
>     /* dividing bar under logo */
>     #header {
>     -moz-box-shadow: 0px 0px 10px #888;
>     -webkit-box-shadow: 0px 0px 10px #888;
>     box-shadow: 0px 0px 10px #888;
>     margin:0px;
>     padding:0;
>     border-bottom:none;
>     width:100%;
>     z-index:100;
>     }
>     /* end logo bar*/

#
>#44. /r/startrek banner
>
>
>###Preview
>
> http://i.imgur.com/kH5JJpB.png
>
>###Code
>
>     
>     /*  announcement banner from /r/startrek */
>     
>     /* use "######" in side */
>     
>     /*---------Announcement banner colors ---------*/
>     
>     .titlebox .usertext-body .md h6:before {
>         /* background-color: #FED259;*/  /*Gold*/
>         /*  background-color: #4379AE;*/    /*Blue*/
>         /*   background-color: #cb4827;*/  /*Red*/
>               background-color: #4C809E; /*unknown name*/
>            color:white;                  /*If banner color is "gold" change this to "black", otherwise leave it "white"*/
>     }
>     
>     .titlebox .usertext-body .md h6 {
>         color: #FED259;    /*Gold*/
>          /*color: #5091D0;*/      /*Blue*/
>         /*color: #000;*/    /*black*/
>               /*color: #2681E9;*/
>     }
>     
>     
>     /*---------Announcement banner ---------*/
>     
>     
>     .titlebox .usertext-body .md h6 {
>         position: absolute;
>         top: 140px;
>         left: 110px;
>         z-index: 100;
>     }
>     .usertext-body .md h6 {
>         line-height: 13px;
>         margin: 0 auto;
>         height: 18px;
>         white-space: nowrap;
>         background: black;
>         /*background: url(%%image%%);*/ /* optional */
>         font-size: 13px;
>         font-weight: normal;
>         text-align: center;
>     /* 2nd px padding sets the width of the banner */
>         padding: 5px 5px 0px 5px;
>         display: block;
>         border-top-right-radius: 7px;
>         border-bottom-right-radius: 7px;
>         border-top-left-radius: 7px;
>         border-bottom-left-radius: 7px;
>     }
>         /*has 'content' (editable below) before the main text in a separate background colour)
>     /*.titlebox .usertext-body .md h6:before {
>         content: " EDIT ME ";
>         font: 10px Helvetica, Verdana, sans-serif;
>         display: inline-block;
>         border-top-left-radius: 7px;
>         border-bottom-left-radius: 7px;
>         position: absolute;
>         left: -10px;
>         top: 0px;
>         height: 13px;
>         padding: 5px 5px 5px 2px;
>         text-align: right;
>         width: 128px;
>         display: table-cell;
>         vertical-align: top;
>         text-shadow: none;}*/
>     
>     /* end startrek banner */

#
>#45. Show last edited timestamp
>
>
>###Preview
>
> http://i.imgur.com/Ji0iibu.png
>
>###Code
>
>     .edited-timestamp[title]:after {
>         content: " (" attr(title) ")";
>         font-size: 90%;
>     }



#
>#46. Replace pagename/subreddit title with an image
>
>
>###Preview
>
> http://i.imgur.com/Hmq00XN.png
>
>###Code
>
>     .pagename a {
>          background: url(%%img_name%%);
>          vertical-align: bottom;
>          display: inline-block;
>          width: 548px /*Edit to your images proportion*/
>          height: 65px;
>          text-indent: -999em;
>     }
>
>If your tabs are floating, you [may need #30](http://www.reddit.com/r/csshelp/wiki/moresnippets#wiki_30._fix_for_floating_pagename.2Ftabs)
>

#
>#47. Hide text on the default reddit logo
>
>
>###Preview
>
> http://i.imgur.com/vOkcRv7.png
>
>###Code
>
>     #header-img.default-header { width: 35px; }
>
> ####Note
>
> If you decide to use a custom logo, don't forget to remove this code!

#
>#48. Change Subreddit's Name
>
>
>###Preview
>
> http://i.imgur.com/nWxCE7A.png
>
>###Code
>
>     .pagename a:after,
>     .titlebox .redditname a:after {
>	     content: "New Name"; /* type the custom name here */
>     }
>
>     .pagename a, .titlebox .redditname a {
>	     font-size: 0!important;
>     }
>
>	     .pagename a:after {
>		     font-size: 18px;
>		     vertical-align: bottom;
>	     }
>
>
>	     .titlebox .redditname a:after {
>	        	font-size: 26px; /*This is the name is the sidebar, so you may need to make it smaller*/
>        	}
>
> 

#
># 49. Center a pagename image in the sidebar
>
>
>###Preview
>
> http://i.imgur.com/sIJEyN2.png
>
>###Code
>
> if you use a pagename image like in #46, you may then want to center it in the sidebar
>
>     .titlebox .redditname a {
>         background-position: center;
>         vertical-align: bottom;
>         width: 300px;
>         background-repeat:no-repeat;
>     }
>

#
>#50. Centers the tabmenu buttons and makes them gradient
>
>
>###Preview
>
> 
>http://i.imgur.com/yfyvqcX.png
>
>###Code
>
>     /*tab menu*/
>     div#header-bottom-left ul.tabmenu{
>     position: absolute;
>     bottom: 0px;
>     left: 350px;
>     /* font-family:Verdana;*/
>     /*text-transform: capitalize;*/
>     font-size: 11px;
>     }
>     .tabmenu li a {
>     /*gradients from /r/beer*/
>     background: -webkit-linear-gradient(white, #A273DC);
>     background: -moz-linear-gradient(white, #A273DC);
>     background: -ms-linear-gradient(white, #A273DC);
>     background: -o-linear-gradient(white, #A273DC);
>     background: linear-gradient(white, #A273DC);
>     /*color: #B6A0C0!important;*/
>     color: #fff!important;
>     border: 0px solid #FFFFFF;
>     }
>     .tabmenu li.selected a {
>     background-color: transparent !important;
>     color: #906BA1 !important;
>     border-color: #000000 !important;
>     border-style: solid;
>     border-width: 0px
>     }
>     .tabmenu li.selected a:hover {
>     background-color: transparent!important;
>     color: #8C4DA9 !important;
>     border-color: #000000 !important;
>     border-bottom: 1px solid #c9c9c9 !important;
>     }
>     .tabmenu li a:hover {
>     background-color: transparent !important;
>     color: #EDE5F1 !important;
>     border-color: #000000 !important;
>     }
>     /*end tabmenu*/
>

#
>#51.  Greentext
>
>
>###Preview
>
> 
>http://i.imgur.com/pdUxaIO.png
>
>###Code
>
>     /*greentext*/
>     .md blockquote {
>         border: 0;
>         margin: 0;
>         color: #789922;
>         display: block;
>         line-height: 0.8
>         }
>     
>     .md blockquote p:before {
>         content: ">";
>         float: left;
>         display: block;
>         }


#
>#52.  Clickable sidebar boxes (**Doesn't work in IE**)
>
>
> Sort of like #26's hover feature, but this one is much cooler.
>
> Made by /u/ggitaliano
>
>
>###Preview
>
> Check out the sidebar at /r/diamotest8 
>
>###Code
> 
>     .side .md h6 { /* list button */
>       position: relative;
>       margin: 0;
>       padding: 5px;
>       background: #F5F5F5;
>       border: 1px solid #DDD;
>       font-size: 12px;
>       color: #111;
>       cursor: pointer;
>     }
>     .side .md h6:after { /* "click to expand" text */
>       content: "click to expand";
>       position: absolute;
>       top: 8px;
>       right: 5px;
>       font-size: 9px;
>       font-weight: normal;
>       color: gray;
>     }
>     .side .md h6 + ul { /* styles (+ hides) the list */
>       position: relative;
>       margin: -35px 0 10px;
>       padding: 28px 0 0;
>       list-style: none;
>       border: 1px solid #DDD;
>       display: none;
>     }
>     .side .md h6:active + ul, /* displays list when button is clicked */
>     .side .md h6 + ul:hover { /* and when hovering over expanded list */
>       display: block;
>     }
>     .side .md h6 + ul li { /* styles list items */
>       position: relative;
>       padding: 5px;
>       border-top: 1px solid #DDD;
>       font-size: 11px;
>     }
> 
> 
> ###Afterwards
>
> Make lists in the sidebar, here is an example:
>
>     ###### Title  
>
>     * Item 1 [link example](http://www.reddit.com)
>     * Item 2
>     * Item 3  
>
> Just make sure that it begins with an `h6` for the title, and then add some bullet points below it.

#
> #Hide Downvote Buttons
>    
>To hide them globally
>
>     .down { display: none; }
>
>To hide them on posts only
>
>     .link .down { display: none; }
>
>To hide them on comments only
>
>     .comment .down { display: none; }
>
>
> Note: This is technically breaking the site and not allowed, but for now the admins have decided to turn a blind eye on it. However, be careful. Also, this does not stop people from downvoting. They can easily do so with RES, other extensions, or even simply opening up their browser console and editing the style in the press of three buttons.
