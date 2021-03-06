<style>
/*Floating Back-To-Top Button*/
    #myBtn {
        position: fixed;
        bottom: 30px;
        float: right;
        right: 10.5%;
        left: 77.25%;
        max-width: 50px;
        width: 200px;
        font-size: 36px;
        border-color: rgba(65, 65, 65, 0.1);
        background-color: rgb(100,100,100,0.6);
       vertical-align: bottom;
        border-radius: 5px;   
        padding: .2px;
    }
/*On Hover Color Change*/
    #myBtn:hover {
        background-color: #15638d;
    }
 
</style>

# INDEX:
* **Texts**
    * [Underline Texts](https://xd.adobe.com/ideas/process/ui-design/use-underline-text-improve-ux/)
	* [Copy/Paste from Word to open edX](#copypaste)
	* [Subtitles](#subtitles)
	* [Missing part and/or attention needed](#missing)
	* [Article quotes and/or tables](#quote)
	* [Ordered/Unordered, Nested, Bold Lists](#lists)
    * [CSS Classes](#link-class)
	* [Announcements Box](#ann-box)
    * [FAQs](#faqs)
*	**Links**
	* [Name Link](#link-name)
    * [CSS Classes](#link-class)
* **Media Embeds**
	* [**MONK (TL;DR the solving problems script)**](#monk)
	
	* **Files and Folders**
		* [Single File](#single-file)
		* [Single Folder](#single-folder)
		* [Multiple Browsable Folders](#multiple-folders)
	* **Images**
		* [Gdrive](#images-gdrive)
	* **Podcasts**
		* [Soundcloud](#soundcloud)
	* **Videos**
		* [Youtube](#youtube)
		* [Facebook](#facebook)
		* [Twitter](#twitter)
		* [Vimeo](#vimeo)
	* **Surveys**
		* [Surveymonkey](#surveymonkey)
		* [Google Forms](#googleforms)


 	 	
<div style="page-break-after: always;"></div>

## Texts
<a name="copypaste"></a>
### Copy/Paste from Word to open edX

1. Copy the text from Word and paste it into [https://word2cleanhtml.com/](https://word2cleanhtml.com/) double check the flags and hit convert to clean html
![](https://drive.google.com/uc?export=view&id=1RDbRlj6XOD5OJUf-NW-YqNoQVCQPjWa-)
2.	Click on *Copy cleaned html to clipboard*
![](https://drive.google.com/uc?export=view&id=1RDbRlj6XOD5OJUf-NW-YqNoQVCQPjWa-)
3. On the backend (AKA Studio of open edx) [https://studio.gchumanrights.org](https://studio.gchumanrights.org) select Raw HTML as the content for the Unit
![](https://drive.google.com/uc?export=view&id=126TP5vZRsQZT3lqEiIIk4LjK2qrPrSJ5)
4. Click on EDIT to obtain the code window 
![](https://drive.google.com/uc?export=view&id=15GEPC6BgmfJ4x2MJ041lMaYp5ISFOXAi)
5. Finally paste the *sanitized code from clipboard* and hit Save 
![](https://drive.google.com/uc?export=view&id=1KoBU6pIPmbRO0rciOrrBDioC_qZiFE8U)

<a name="subtitles"></a>
### Subtitles
##### IE [Hate Speech and Hate Crime]:
![](https://drive.google.com/uc?export=view&id=1muc3_jzzjD-Zb33aBCGyi-D-Syw8nmpK)
##### Code:
<pre>&lt;p <span style="color: #ff40ff;">class="subtitle_page_programme"</span>>Hate Speech and Hate Crime &lt;/p></pre>

<a name="missing"></a>
## Missing part and/or attention needed

Whenever you find some texts missing or some incomplete part it will be nice to use the appropriate *class* so it can be double checked easily
##### IE:
![](https://drive.google.com/uc?export=view&id=12fQQ1ON7xw2SbjF-2hDGVkIuhZVQUjF6)
##### Code:
<pre class="default prettyprinted prettyprint">&lt;p>
&lt;span <span style="color: #ff40ff;">class="themissing"</span>>Freedom of expression on Internet: https://www.coe.int/en/web/human-rights-channel/-/free-expression-on-the-internet&lt;/span>
&lt;/p></pre>

<a name="quote"></a>
## Article quotes and/or tables

##### IE:
![](https://drive.google.com/uc?export=view&id=1cj6nT6nXbieG-7-938xlygNIxI4YLqsC)
##### Code:
```html
<table border="1" cellspacing="0" cellpadding="0" class="table-articles">
    <tbody>
        <tr>
            <td width="100%" valign="top">
                <p>
                    <a name="_Hlk524902982">
                        Art. 17 Right to property
                    </a>
                </p>
                <p>
                    1. Everyone has the right to own, use, dispose of and
                    bequeath his or her lawfully acquired possessions. No one
                    may be deprived of his or her possessions, except in the
                    public interest and in the cases and under the conditions
                    provided for by law, subject to fair compensation being
                    paid in good time for their loss. The use of property may
                    be regulated by law in so far as is necessary for the
                    general interest.
                </p>
                <p>
                    2. Intellectual property shall be protected.
                </p>
            </td>
        </tr>
    </tbody>
</table>
```
**The Title of the table is done with an anchor tag**
	<pre class="default prettyprinted prettyprint">&lt;a <span style="color: #ff40ff;">name="putanamehere"</span>>Art. 17 Right to property&lt;/a></pre>


<a name="lists"></a>
## Ordered/Unordered, Nested, Bold Lists
### Ordered Lists
#### IE of ordered list
<img src="https://drive.google.com/uc?export=view&id=1Id8QLdBzdQUZzlHXS2AxOK5aApPvYowz" alt="image_description" />

<pre>
&lt;ul <span style="color: #ff40ff;">class="number_list"</span>>
	&lt;li>one&lt;/li>
	&lt;li>two&lt;/li>
	&lt;li>three&lt;/li>
&lt;/ul>
</pre>

### Alphabetical Lists
#### IE of alphabetical list
<img src="https://drive.google.com/uc?export=view&id=1r4gIjEVso86aDlkUFuBY-Y2WfwxzFnsf" alt="image_description" />

<pre>
&lt;ul <span style="color: #ff40ff;">class="letter_list"</span>>
	&lt;li>one&lt;/li>
	&lt;li>two&lt;/li>
	&lt;li>three&lt;/li>
&lt;/ul>
</pre>

### Unordered Lists
#### IE of Unordered list
<img src="https://drive.google.com/uc?export=view&id=1p18T-dn2vxsOIwF59xD01b2nZbJir_N-" alt="image_description" />

<pre>
&lt;ul <span style="color: #ff40ff;">class="lista_con_pallini"</span>>
	&lt;li>one&lt;/li>
	&lt;li>two&lt;/li>
	&lt;li>three&lt;/li>
&lt;/ul>
</pre>

### Nested Lists
#### IE of Nested list

<img src="https://drive.google.com/uc?export=view&id=16vaNudpdfv4j2XJG96xxJ_X6ThGzhNks" alt="image_description" />

<pre>
&lt;ul class="lista_con_pallini">
    &lt;li>List of Lists
        <span style="color: #ff40ff;">&lt;ul class="lista_con_pallini"></span>
            &lt;li>Unsorted&lt;/li>
            &lt;li>Unfortunate&lt;/li>
            &lt;li>Unsorted&lt;/li>
            &lt;li>Unfortunate&lt;/li>
        &lt;/ul>
    &lt;/li>
    &lt;li>Unsorted&lt;/li>
    &lt;li>Unfortunate&lt;/li>
&lt;/ul>
</pre>

### Bold Lists
#### IE of Bold and Nested Lists 

<img src="https://drive.google.com/uc?export=view&id=1EL-yrOUNui5_F07HU1DkN-Fm7xpllQWf" alt="image_description" />

<pre>
&lt;ul <span style="color: #ff40ff;">class="number_list_bold"</span>&gt;
	&lt;li&gt;Trafficking needs an element of movement, but not a movement across
	        borders.&lt;/strong&gt;
		&lt;br&gt;<span style="color: #ff40ff;">&lt;span&gt;</span>There are two important points here:&lt;/span&gt;&lt;br&gt;
		&lt;ul class="lista_con_pallini"&gt;
		&lt;li&gt;
			&lt;span&gt;Does trafficking need movement? There is an evolving debate on the
			necessity of movement in the crime of trafficking. Recently there has been
			a move to conflate trafficking with slavery and forced labour (both of
			which do not need movement). Though the &lt;em&gt;Travaux Preparatories&lt;/em&gt; for
			the Palermo Protocol (the official record of the negotiation during the
			drafting) note that the drafters saw an element of movement as compulsory
			for the definition, more recently the US government’s Trafficking in
			Person’s office and influential NGOs (such as Kevin Bales Free the
			Slaves and Anti-Slavery), all regard trafficking as a part of ‘modern
			day slavery.’
			&lt;br&gt;For details of this debate see: Janie A. Chuang. 2014. “Exploitation
		Creep and the Unmaking of Human Rights Law.” &lt;em&gt;American Journal of International Law&lt;/em&gt; 108: 609-649.
			&lt;/span&gt;
		&lt;/li&gt;
		&lt;li&gt;
			<span style="color: #ff40ff;">&lt;span&gt;</span>Trafficking within a country. Mostly media and counter trafficking
			represent trafficked victims as non citizens, as people who were taken
			across a border for exploitation. While this is the most common form of
			trafficking in Southeast Asia, there are trafficking pathways which are
			internal to a country. People are still trafficked from the countryside to
			the city, for example child domestic workers. Indigenous and minority
			groups are also vulnerable to internal trafficking. Another case is during
			disasters as there are concerns that people can be trafficked out of
			humanitarian camps.&lt;/span&gt;
		 &lt;/li&gt;
&lt;/ul&gt;
</pre>

<a name="ann-box"></a>
## Announcements Box
### Colored Announcements boxes

Announcements boxes are useful when you want to make a bold announcement.

#### IE of Colored announcements boxes:
<img src="assets/imgs/announcements-box.png" alt="image_description" />

#### Code:
```html
<style>
.announcements-box {
    padding: 20px;
    background-color: #f44336;
    color: white;
    transition: opacity 0.6s;
    margin-bottom: 15px;
    min-height: 50px;
    border-radius: 4px;
    font-size: 18px;
    vertical-align: center;
}

.closebtn {
    margin-left: 15px;
    color: fff;
    font-weight: bold;
    float: right;
    font-size: 22px;
    line-height: 20px;
    cursor: pointer;
    transition: 0.3s;
}

.closebtn: hover {
    color: #75716e;
}

.primary {
    background: #75716e;
}

.info {
    background-color: #009fe3;
}

.success {
    background: #15CD72;
}

.danger {
    background: #e6553d;
}

.warning {
    background: #f9bd00;
}

.muted {
    background: #ECECEC;
    color: #75716e;
}
</style>

<div class="announcements-box primary">
    <span class="closebtn" onclick="this.parentElement.style.display='none';">×</span>
    <strong>PRIMARY</strong><br><br>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam ultricies quis arcu eget commodo. Etiam tempor lacus lorem, et ullamcorper odio interdum id. Morbi odio augue, porttitor eu posuere at, consequat eu augue. 
</div>
<p class="margin_bottom_20"></p>
<div class="announcements-box info">
    <span class="closebtn" onclick="this.parentElement.style.display='none';">×</span>
    <strong>INFO</strong><br><br>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam ultricies quis arcu eget commodo. Etiam tempor lacus lorem, et ullamcorper odio interdum id. Morbi odio augue, porttitor eu posuere at, consequat eu augue. 
</div>
<p class="margin_bottom_20"></p>
<div class="announcements-box success">
    <span class="closebtn" onclick="this.parentElement.style.display='none';">×</span>
    <strong>SUCCESS</strong><br><br>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam ultricies quis arcu eget commodo. Etiam tempor lacus lorem, et ullamcorper odio interdum id. Morbi odio augue, porttitor eu posuere at, consequat eu augue. 
</div>
<p class="margin_bottom_20"></p>
<div class="announcements-box warning">
    <span class="closebtn" onclick="this.parentElement.style.display='none';">×</span>
     <strong>WARNING</strong><br><br>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam ultricies quis arcu eget commodo. Etiam tempor lacus lorem, et ullamcorper odio interdum id. Morbi odio augue, porttitor eu posuere at, consequat eu augue. 
</div>
<p class="margin_bottom_20"></p>
<div class="announcements-box danger">
    <span class="closebtn" onclick="this.parentElement.style.display='none';">×</span>
     <strong>DANGER</strong><br><br>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam ultricies quis arcu eget commodo. Etiam tempor lacus lorem, et ullamcorper odio interdum id. Morbi odio augue, porttitor eu posuere at, consequat eu augue. 
</div>
<p class="margin_bottom_20"></p>
<div class="announcements-box muted">
    <span class="closebtn muted" onclick="this.parentElement.style.display='none';">×</span>
     <strong>MUTED</strong><br><br>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam ultricies quis arcu eget commodo. Etiam tempor lacus lorem, et ullamcorper odio interdum id. Morbi odio augue, porttitor eu posuere at, consequat eu augue. 
</div>
```
<a name="faqs"></a>
## FAQs for edX Courses
### The working faqs
```html
<style>
    .xblock .xblock h2 {
        font-weight: 300 !important;
        text-transform: initial;
        color: #75716e !important;
        font-size: 24px;
    }  
    .h2faq{
        font-size: 20px !important;
        font-weight: 300 !important;
        letter-spacing: 0px !important;
        line-height: 30px !important;
    }
    .h3faq{
        font-size: 16px !important;
        font-weight: 300 !important;
        letter-spacing: 0px !important;
        line-height: 22px !important;
        color: #646464 !important
    }
</style>  
<div class="mod_faqpage description_page_programme_no_border no_margin_bottom block">
        <article class="first even">
            <h2 class="h2faq">Enrolment</h2>

            <!--<section class="first even">
                <h3 class="h3faq" id="how-do-i-enrol-in-the-course-44aac414">How do I enrol in the course?</h3>

                <div class="ce_text block">
                    <p>In order to enrol, please follow the instructions on our “<a href="education/e-learning/moocs/monitoring-the-human-rights-of-lgbti-persons/how-to-enrol.html">How to enrol</a>” webpage . This will then lead you to the OpenEdX course page. Once you are there, you can start the enrolment process by clicking the "enrol" button.</p>
                </div>

                
            </section>-->

            <section class="last odd">
                <h3 class="h3faq" id="is-there-a-selection-procedure-to-participate-in-the-course-5a9b94ac">Is there a selection procedure to participate in the course?</h3>

                <div class="ce_text block">
                    <p>The course is a MOOC (Massive Open Online Course), which means we do not select participants on any basis. Rather, we welcome anyone who is interested in learning more about the topic to enrol and participate for free.</p>
                </div>

                
            </section>

           
        </article>
        
        <article class="odd">
            <h2 class="h2faq">Fees</h2>

            <section class="first even">
                <h3 class="h3faq" id="i-would-like-to-know-if-the-course-is-free-or-if-some-parts-are-to-be-paid-4b30d678">I would like to know if the course is free or if some parts are to be paid</h3>

                <div class="ce_text block">
                    <p>Our course is a MOOC (Massive Open Online Course), which means all components are open and totally free for anyone.</p>
                </div>

                
            </section>

            <section class="last odd">
                <h3 class="h3faq" id="i-would-like-to-know-if-the-course-is-free-or-if-some-parts-are-to-be-paid-148-27d18db9">Do I need to pay any fee to attend the course?</h3>

                <div class="ce_text block">
                    <p>There are no registration or tuition fees. </p>
                </div>

                
            </section>

           
        </article>
        

        <article class="odd">
            <h2 class="h2faq">Accessibility</h2>

            <section class="first last even">
                <h3 class="h3faq" id="is-the-course-accessible-to-persons-with-disabilities-c132662c">Is the course accessible to persons with disabilities?</h3>

                <div class="ce_text block">
                    <p class="margin_bottom_20">We want all participants in our courses to enjoy a great learning experience and we strive to always improve accessibility. Each week of the course includes one or two video lectures with accompanying transcripts and reading materials. The texts are in PDF format, work at low bandwidths, are printable and can be zoomed to the desired size. Some readings may include pages from accessible websites. This makes all of them accessible to those who use assistive technology software such as screen readers. Likewise, weekly discussions and module quizzes can be completed through our platform which is accessible, for example, to people who use speech input, keyboard accessible controls or text to speech tools. For more details please visit <a class="titolo_gc_europe" href="https://www.edx.org/accessibility">EdX Website Accessibility Policy</a> &nbsp;</p>
                </div>

                
            </section>

           
        </article>

        <article class="even">
            <h2 class="h2faq">Structure and content</h2>
            
            <section class="first last even">
                <h3 class="h3faq" id="is-there-a-schedule-for-the-course-or-is-it-self-directed-e2186c8d">Is there a schedule for the course?</h3>

                <div class="ce_text block">
                    <p>The course is self-paced so participants can study in their own time. However, in order to enhance peer learning, interactive participation and self-assessment, weekly topics and discussions as well as module quizzes are proposed at set dates. In any case, they are all open until the end of the course to facilitate access and completion at any preferred time. For a detailed description of the schedule check the <a href="https://gchumanrights.org/education/e-learning/moocs/fundamental-rights-of-the-european-union/course-outline.html" target="_blank">course outline page</a> on our website.</p>
                </div>

                
            </section>


            <section class="first last even">
                <h3 class="h3faq" id="is-there-a-schedule-for-the-course-or-is-it-self-directed-e2186c8d">I have a commitment in week 2. Would it be possible to work on it the following weeks?</h3>

                <div class="ce_text block">
                    <p>As the course is self-paced, the workload can be shifted from one week to the other. </p>
                    <!-- Even the quizzes can be taken in a one week span, so that every participant can adjust it to his/her personal commitments. -->
                </div>

                
            </section>
            <!--<section class="first last even">
                <h3 class="h3faq" id="is-there-a-schedule-for-the-course-or-is-it-self-directed-e2186c8d">How do I take part in discussions?</h3>

                <div class="ce_text block">
                    <p>Discussions are based on an initial question/prompt that refers to the content studied in a particular week and that usually gives you the opportunity to discuss, share examples, propose ideas, and interact with other participants. Participation in discussions is part of the learning process for all. Therefore, we trust each active participant will make meaningful contributions (so please note that a simple answer such as "I agree" will not be considered valid for the purpose of earning the certificate of participation). Due to the large number of participants, it might be difficult to follow all inputs, but you can easily search the discussion forum with keywords, names, issues, etc. Responses are also nested so that if you respond to another participant, you'll see the flow of your exchanges immediately below the initial input. At times it might be useful to create a group discussion if participants are particularly interested in further exchanges on a specific sub-issue. In such cases, the coordinating team will set up another discussion and interested participants will be able to join this one too.</p>
                </div>

                
            </section>
            <section class="first last even">
                <h3 class="h3faq" id="is-there-a-schedule-for-the-course-or-is-it-self-directed-e2186c8d">Quizzes</h3>

                <div class="ce_text block">
                    <p>Quizzes are foreseen at the end of each Module in order for you to check your understanding and progress. They are based on 5 questions and require a score of 4/5 to pass. They consist of different types of questions (true/false; yes/no; multiple choice; multiple answer) and once open, they remain available until the end of the course. You can have unlimited attempts and can see what answers you got wrong/right. However, for a more effective and satisfactory learning experience we warmly encourage you to take the quizzes after having prepared for them properly and not at random. 

</p>
                </div>

                
            </section>
            <section class="first last even">
                <h3 class="h3faq" id="is-there-a-schedule-for-the-course-or-is-it-self-directed-e2186c8d">What are the requirements to complete the course? </h3>

                <div class="ce_text block">
                    <p>To successfully complete the course students must take part in 4 weekly discussions and pass 3 quizzes.</p>
                </div>

                
            </section>-->


           
        </article>

        

        <article class="last even">
            <h2 class="h2faq">Certificate of participation</h2>

            <section class="first last even">
                <h3 class="h3faq" id="what-do-i-need-to-do-to-get-the-certificate-of-participation-c1ac8fc6">If I complete the Course will I get the Certificate?</h3>

                <div class="ce_text block">
                    <p>At the end of the course you will not receive a certificate of participation.

</p>

                    <p>&nbsp;</p>
                </div>

                
            </section>

           
        </article>
    </div>

```

## Links&Span

<a name="link-name"></a>

### Link Name


<p>The <strong>A element</strong> defines an anchor.</p>

<p>You can create a link to a named anchor by using the <span class="SoAttr">name</span> attribute (or the <a href="../attribute/id.html">id attribute</a>).</p>

<p>When linking within the same document, the A element is set as follows.</p>



<pre>

&lt;a href="#Anchorname">linked text&lt;/a>

(Target point) 
&lt;a name="Anchorname">a named anchor&lt;/a>

</pre>

<a name="link-class"></a>
### CSS Classes

Usually you would not use a class for the anchor tag, but it may happen that you want to use different color for specific regions:

<pre>
&lt;p&gt;&lt;span class="<span style="color: #009fe3;">titolo_gc_europe</span>"><span style="color: #009fe3;">EUROPE</span>&lt;/span&gt;&lt;/p>
&lt;p&gt;&lt;span class="<span style="color: #69c8f3;">titolo_gc_south_east_europe</span>"><span style="color: #69c8f3;">SOUTH EAST EUROPE</span>&lt;/span&gt;&lt;/p>
&lt;p&gt;&lt;span class="<span style="color: #e6553d;">titolo_gc_caucasus</span>"><span style="color: #e6553d;">CAUCASUS</span>&lt;/span&gt;&lt;/p>
&lt;p&gt;&lt;span class="<span style="color: #f9bd00;">titolo_gc_africa</span>"><span style="color: #f9bd00;">SOUTH AFRICA</span>&lt;/span&gt;&lt;/p>
&lt;p&gt;&lt;span class="<span style="color: #ed6ea7;">titolo_gc_asia_pacific</span>"><span style="color: #ed6ea7;">ASIA PACIFIC</span>&lt;/span&gt;&lt;/p>
&lt;p&gt;&lt;span class="<span style="color: #be97c5;">titolo_gc_latin_america</span>"><span style="color: #be97c5;">LATIN AMERICA</span>&lt;/span&gt;&lt;/p>
&lt;p&gt;&lt;span class="<span style="color: #f08c22;">titolo_gc_arab</span>"><span style="color: #f08c22;">ARAB WORLD</span>&lt;/span&gt;&lt;/p>
</pre>

## Media Embeds
Usually you will have to embed different kind of media: Images, Videos, Podcasts and Files.
Every hosting has it own set of rules, that can change in time so take these instructions with a grain of salt. The vade mecum will be updated regularly and will take changes into account: if you find some code not working please promptly report it ^_^

### MONK (TL;DR the solving problems script)
<a name="monk"></a>
Monk is a quick tool lets you easily paste a shareable link from gdrive and obtain the code to be used on open edX for:
	
* Single File
* Single File Landscape
* Single Folder - Grid View
* Single Folder - List View
* Browseable Folder
* Image

1. Upload your file to GDrive
2. Right click on the file from Gdrive and click on *Get shareable link*
![](https://drive.google.com/uc?export=view&id=1OiUlcy83eugjcaXnApGmlEwUYLefhl6g)
3. Paste the shared link on [https://gchumanrights.org/monk/monk.php](https://gchumanrights.org/monk/monk.php)
<img src="https://drive.google.com/uc?export=view&id=1YhGdjFd9g6mr6XRhGSPMAzygLSz2vlYi" alt="image_description" />
3. Choose the type of link you need and click on the SEND button
<img src="https://drive.google.com/uc?export=view&id=1FY7R7lS1AwDtzSCXC3iQgG3UOS3naktT" alt="image_description" />
4. Click on the COPY button to get the markup needed on edX
<img src="https://drive.google.com/uc?export=view&id=1lJxLDnZI7o6jue1RR0y8S8jSDv7TG9Y0" alt="image_description" />

### Files & Folders
<a name="single-file"></a>
#### Single file
1. Upload your file to GDrive
2. Right click on the file from Gdrive and click on *Get shareable link*
![](https://drive.google.com/uc?export=view&id=1OiUlcy83eugjcaXnApGmlEwUYLefhl6g)
3. Paste the shared link on notepad or wherever, it should look similar to this:
<pre>https://drive.google.com/open?id=<span style="color: #ff40ff;">1Axs4BGN3ywuYIrlHJ50K6O675CV5uqyN</span></pre>
4. Copy the highlighted part (whatever comes after id=) and check if the file orientation (portrait or landscape):
	* For **portrait** file you can use this code and replace the id (<span style="color: #ff40ff;">highlighted</span>) with the one you've just copied
	
		<pre>
		&lt;div class="box_vertical_a4_container">
	        &lt;iframe class="box_vertical_a4" src="https://drive.google.com/file/d/<span style="color: #ff40ff;">1Axs4BGN3ywuYIrlHJ50K6O675CV5uqyN</span>/preview">&lt;/iframe>
	   &lt;/div>
		</pre>
	
	* For **landscape** file you can use this code and replace the id (<span style="color: #ff40ff;">highlighted</span>) with the one you've just copied
	
		<pre>
		&lt;div class="box_horizontal_a4_container">
	        &lt;iframe class="box_horizontal_a4" src="https://drive.google.com/file/d/<span style="color: #ff40ff;">1Axs4BGN3ywuYIrlHJ50K6O675CV5uqyN</span>/preview">&lt;/iframe>
	   &lt;/div>
		</pre>
		
5. Results should look similar to those:
![](https://drive.google.com/uc?export=view&id=1zXVga01kfAbQPZhHxmdH-D_lPjaj764r)
![](https://drive.google.com/uc?export=view&id=1YA3eIGVLerxY1Bx0g3pJiHyYbresALEv)

<a name="single-folder"></a>
#### Single Folder
1. Create your folder on GDrive (it should contain at least two files otherwise check [Single File](#single-file))
2. Right click on the folder from Gdrive and click on *Get shareable link*
![](https://drive.google.com/uc?export=view&id=19Db85K2po9xydgMd4GsdiKL-1v7buMID)
3. Paste the shared link on notepad or wherever, it should look similar to this:
<pre>https://drive.google.com/open?id=<span style="color: #ff40ff;">19Db85K2po9xydgMd4GsdiKL-1v7buMID</span></pre>
4. Copy the highlighted part (whatever comes after id=)):
	* For **grid view** (when there're few files) you can use this code and replace the id (<span style="color: #ff40ff;">highlighted</span>) with the one you've just copied
	
		<pre>
		&lt;iframe src="https://drive.google.com/embeddedfolderview?id=<span style="color: #ff40ff;">FOLDER-ID</span>#grid" style="width:100%; height:600px; border:0;">&lt;/iframe>		</pre>
	
	* For **list view** (when there're many files) you can use this code and replace the id (<span style="color: #ff40ff;">highlighted</span>) with the one you've just copied
	
		<pre>
		&lt;iframe src="https://drive.google.com/embeddedfolderview?id=<span style="color: #ff40ff;">FOLDER-ID</span>#list" style="width:100%; height:600px; border:0;">&lt;/iframe>
		</pre>
		

		
5. Results should look similar to those:
![](https://drive.google.com/uc?export=view&id=1wen0c5MIx2mXSzFlh78foja59n-jILWS)
![](https://drive.google.com/uc?export=view&id=1NmNzWTGxy1-JFQ7QQGR7-HTfIsx8z_c1)

<a name="multiple-folders"></a>
#### Multiple Browsable Folders
1. Create your folder with sub-folder(s) on GDrive 
2. Right click on the folder from Gdrive and click on *Get shareable link*
![](https://drive.google.com/uc?export=view&id=19Db85K2po9xydgMd4GsdiKL-1v7buMID)
3. Paste the shared link on notepad or wherever, it should look similar to this:
<pre>https://drive.google.com/open?id=<span style="color: #ff40ff;">1ZjrJK2kmBiLDZAHdt7AhZCFDMmFQWE5s</span></pre>
4. Copy the highlighted part (whatever comes after id=)
	
	<pre>&lt;div class="box_horizontal_a4_container">
		&lt;iframe class="box_horizontal_a4" src="https://gchumanrights.org/edxtools/z_gdrive_viewer.php?ID=<span style="color: #ff40ff;">1aAABmOzQV9IVp_lTOkd42_Rl3bgHjpUL</span>">&lt;/iframe>
	&lt;/div></pre>
5. Result should look similar to this:
![](https://drive.google.com/uc?export=view&id=1SHQFO4qAk9UTkT8C9MXupXBygG5RpeWE)

### Images
<a name="images-gdrive"></a>
#### Gdrive
#### Single file
1. Upload your file to GDrive
2. Right click on the file from Gdrive and click on *Get shareable link*
![](https://drive.google.com/uc?export=view&id=1L1aU8fWbn4ywFh1rX8M3Giu3oNn_FQkS)
3. Paste the shared link on notepad or wherever, it should look similar to this:
<pre>https://drive.google.com/open?id=<span style="color: #ff40ff;">1L1aU8fWbn4ywFh1rX8M3Giu3oNn_FQkS</span></pre>
4. Copy the highlighted part (whatever comes after id=) and check if the file orientation (portrait or landscape):
For **portrait** file you can use this code and replace the id (<span style="color: #ff40ff;">highlighted</span>) with the one you've just copied
	

	<pre>
		&lt;img src="https://drive.google.com/uc?export=view&id=<span style="color: #ff40ff;">1aAABmOzQV9IVp_lTOkd42_Rl3bgHjpUL</span>" alt="image_description" />
	</pre>	
	
			
5. Result should look similar to this:
![](https://drive.google.com/uc?export=view&id=1DR04qS1rvwXXFXKYmPBlzWqgQp2qQpnN)



### Podcasts
<a name="soundcloud"></a>
#### Soundcloud
##### IE podcast to be embedded [https://soundcloud.com/taleofus/caribou-cant-do-without-you-tale-of-us-mano-le-tough-remix](https://soundcloud.com/taleofus/caribou-cant-do-without-you-tale-of-us-mano-le-tough-remix)
**1. Click on Share button and then on Embed:**

<img src="https://drive.google.com/uc?export=view&id=156-eY4r3cJXJQu0CWUED5agmJnqSrk76" height="500" />

**2. Copy the code for classic Embed [second option]**
<pre>&lt;iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/166083001&color=%23ff5500&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true">&lt;/iframe></pre>

**3. Paste the code on open edX:**

<pre>&lt;iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/166083001&color=%23ff5500&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true">&lt;/iframe></pre>



### Videos
<a name="youtube"></a>
#### YouTube
Youtube is the video providers for the online courses because of its deep integration with edX.
To correctly post a video from youtube to edX you should have: URL of the video and it subtitles
###### How to get the subtitles 
1. Login to youtube (username and password were delivered by email)
2. Go to this link [https://studio.youtube.com/channel/UC7xO-4Vs8EnTdwrUg3rSzug/videos/upload] (https://studio.youtube.com/channel/UC7xO-4Vs8EnTdwrUg3rSzug/videos/upload)
3. Click on the title of the video you want to embed
<img src="https://drive.google.com/uc?export=view&id=1nrGcmtoo7SDGzWB8BEg5jpLXWo6IF9sl" alt="image_description" />
4. Click on the left menu *Transcriptions*
<img src="https://drive.google.com/uc?export=view&id=1G3WIQni3Hbqa_d97LeYWmJ0sgeMFYVdn" alt="image_description" />
5. On the right side click on the English Automatic translation
<img src="https://drive.google.com/uc?export=view&id=1CbVwRI67ejVYUvbji1r3s2jWjYpkRmtk" alt="image_description" /> 
6. On the new open window click on actions and select SRT
<img src="https://drive.google.com/uc?export=view&id=1O4GawCv9HAl0byvTzTr_BN-uuYuEY3qi" alt="image_description" />
7. Download the subtitles and be ready to upload it to edX


###### How to get the Video URL 
1. Login to youtube (username and password were delivered by email)
2. Go to this link [https://studio.youtube.com/channel/UC7xO-4Vs8EnTdwrUg3rSzug/videos/upload] (https://studio.youtube.com/channel/UC7xO-4Vs8EnTdwrUg3rSzug/videos/upload)
3. Click on the title of the video you want to embed
<img src="https://drive.google.com/uc?export=view&id=1nrGcmtoo7SDGzWB8BEg5jpLXWo6IF9sl" alt="image_description" />
4. Click on the right side copy video URL
<img src="https://drive.google.com/uc?export=view&id=1HfPD-7K-3nLyAjhuFYto6HdKH8iB9xqQ" alt="image_description" />


###### Embeding on edX
1. As the unit content select Video
<img src="https://drive.google.com/uc?export=view&id=1Y6hc5XRzSnrmoGNDK0vkR5Xe1tc60FzV" alt="image_description" />
2. Once the unit is loaded click on EDIT
<img src="https://drive.google.com/uc?export=view&id=1u-l7_QxCJMrQO4dOAwpxy50-1WWJLpHH" alt="image_description" />
3. While on the default edit tab please paste the youtube url
<img src="https://drive.google.com/uc?export=view&id=1vA7oBRgHUoaATC8P9VH-pi14MqoQ_SA5" alt="image_description" />
4. After that click on Upload New Transcript
<img src="https://drive.google.com/uc?export=view&id=14u2SK7vxLDCpccBKlh_sFRKyOYk9V11D" alt="image_description" />
6. Click on Save [Left bottom Corner]



<a name="facebook"></a>
#### Facebook
##### IE video to be embedded [https://www.facebook.com/eiuc.venice/videos/1158241700993405/](https://www.facebook.com/eiuc.venice/videos/1158241700993405/)

**1. Click on the 3 horizontal dots and select Embed:**
![](https://drive.google.com/uc?export=view&id=1s29pqeBGRYA7AU5Bw3X2UhphcPwGuKGh)
**2. Copy the code starting with &lt;iframe ...:**
![](https://drive.google.com/uc?export=view&id=1yfv_am7hcrufw7I9JATfrLvkexVJcvAB)
it should be similar to this:

<pre>&lt;iframe <span style="color: #ff40ff;">src="https://www.facebook.com/plugins/video.php?href=https%3A%2F%2Fwww.facebook.com%2Feiuc.venice%2Fvideos%2F1158241700993405%2F&show_text=0&width=560"</span>  width="560"height="315" style="border:none;overflow:hidden"scrolling="no" frameborder="0" allowTransparency="true" allowFullScreen="true">&lt;/iframe></pre>

**3. Code to be pasted in open edX [the only part to be kept out of the copied code is the highlighted src attribute]:**

<pre>
&lt;div class="video169_container">
&lt;iframe class="video169" <span style="color: #ff40ff;">src="https://www.facebook.com/plugins/video.php?href=https%3A%2F%2Fwww.facebook.com%2Feiuc.venice%2Fvideos%2F1930785920278482%2F&show_text=0&width=560"</span> frameborder="0" allowfullscreen="">&lt;/iframe>
&lt;/div>
</pre>

<a name="twitter"></a>
#### Twitter
##### IE video to be embedded [https://twitter.com/WhiteCodeCentre/status/1077442937884164096](https://https://twitter.com/WhiteCodeCentre/status/1077442937884164096)

**1. Click on the chevron select Copy link to Tweet:**
![](https://drive.google.com/uc?export=view&id=1UUgGSqjGp_Go5GcA2pXRY5x_ujqJsb_g)

**2. The URL should be similar to this:**
<pre>https://twitter.com/WhiteCodeCentre/status/<span style="color: #ff40ff;">1077442937884164096</span></pre>

**3. Code to be pasted in open edX [the only part to be kept out of the copied URL is the one highlighted (video ID) which has to be modified accordingly on the code below]:**

<pre>
&lt;div class="video169_container">
&lt;iframe class="video169" src="https://twitter.com/i/videos/<span style="color: #ff40ff;">1077442937884164096</span>" frameborder="0" allowfullscreen="">&lt;/iframe>
&lt;/div>
</pre>


<a name="vimeo"></a>
#### Vimeo
##### IE video to be embedded [https://vimeo.com/207085016](https://vimeo.com/207085016)

**1. Click on the paper ariplane Share button:**
![](https://drive.google.com/uc?export=view&id=1ruW6rklSGGLqiXuypkyVaCnR3BMPPiil)
**2. Copy the code for Embed:**
<pre>&lt;iframe src="https://player.vimeo.com/video/<span style="color: #ff40ff;">207085016</span>"</span> width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen>&lt;/iframe>
&lt;p>&lt;a href="https://vimeo.com/207085016">Global Campus Human Rights Journal - Viljoen&lt;/a> from &lt;a href="https://vimeo.com/eiuc">EIUC - Global Campus&lt;/a> on &lt;a href="https://vimeo.com">Vimeo&lt;/a>.&lt;/p></pre>

**3. Code to be pasted in open edX [the only part to be kept out of the copied URL is the one highlighted (video ID) which has to be modified accordingly on the code below]:**

<pre>
&lt;div class="video169_container">
&lt;iframe class="video169" src="https://player.vimeo.com/video/<span style="color: #ff40ff;">207085016</span>" frameborder="0" allowfullscreen="">&lt;/iframe>
&lt;/div>
</pre>

### Surveys
<a name="surveymonkey"></a>
#### SurveyMonkey
##### IE Survey to be embedded [https://www.surveymonkey.com/r/NFL6PDT](https://www.surveymonkey.com/r/NFL6PDT)

**1. Click on the paper ariplane Share button:**
![](https://drive.google.com/uc?export=view&id=1afbJWO_vPZPl04SkabOhwyQaWFOqRWue)
**2. Click on Web Link 1**
![](https://drive.google.com/uc?export=view&id=1fvJGwzNnBRzqmi_SuhjVAAvEj8fG4EwF)
**3. Click on Copy**
![](https://drive.google.com/uc?export=view&id=1LrojwRx-9GkLEkWfdLDIGQo6syo02R_e)
**4. Replace the highlighted src with the copied one**
<pre>
&lt;p>&lt;iframe src="<span style="color: #ff40ff;">https://www.surveymonkey.com/r/T25DVBR</span>" height="500px" width="100%">&lt;/iframe>&lt;/p>
</pre>

<a name="googleforms"></a>
#### Google Forms
##### IE Survey to be embedded [https://forms.gle/rpdGz8UPiCvXcFJj9)

**1. Click on the SEND button and the choose the embed icon:**
![](https://drive.google.com/uc?export=view&id=1dx5g65fE2e6lSfUunKBHyZOK0GWsytX8)
**2. Copy the Code on Embed HTML**

**3. Replace the highlighted src with the copied one**
<pre>
&lt;p>&lt;iframe src="<span style="color: #ff40ff;">https://docs.google.com/forms/d/e/1FAIpQLSeLoABZkKjglKUydauNag9nv6bDx0RT7bXv-7AoWnrL1zQ2jA/viewform?embedded=true</span>" width="100%" height="700" frameborder="0" marginheight="0" marginwidth="0">&lt;/iframe>&lt;/p>
</pre>

<button id="myBtn"><a href="#top" style="color: white; text-decoration: none; vertical-align:bottom;">^</a></button>
<!-- rev 10 - Initial Github release-->
##### 23 Apr. 2020 - Initial Github release