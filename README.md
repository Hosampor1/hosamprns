## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/Hosampor1/hosamprns/edit/main12/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Hosampor1/hosamprns/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

Markdown: Basics
================

<ul id="ProjectSubmenu">
    <li><a href="/projects/markdown/" title="Markdown Project Page">Main</a></li>
    <li><a class="selected" title="Markdown Basics">Basics</a></li>
    <li><a href="/projects/markdown/syntax" title="Markdown Syntax Documentation">Syntax</a></li>
    <li><a href="/projects/markdown/license" title="Pricing and License Information">License</a></li>
    <li><a href="/projects/markdown/dingus" title="Online Markdown Web Form">Dingus</a></li>
</ul>


Getting the Gist of Markdown's Formatting Syntax
------------------------------------------------

This page offers a brief overview of what it's like to use Markdown.
The [syntax page] [s] provides complete, detailed documentation for
every feature, but Markdown should be very easy to pick up simply by
looking at a few examples of it in action. The examples on this page
are written in a before/after style, showing example syntax and the
HTML output produced by Markdown.

It's also helpful to simply try Markdown out; the [Dingus] [d] is a
web application that allows you type your own Markdown-formatted text
and translate it to XHTML.

**Note:** This document is itself written using Markdown; you
can [see the source for it by adding '.text' to the URL] [src].

  [s]: /projects/markdown/syntax  "Markdown Syntax"
  [d]: /projects/markdown/dingus  "Markdown Dingus"
  [src]: /projects/markdown/basics.text


## Paragraphs, Headers, Blockquotes ##

A paragraph is simply one or more consecutive lines of text, separated
by one or more blank lines. (A blank line is any line that looks like
a blank line -- a line containing nothing but spaces or tabs is
considered blank.) Normal paragraphs should not be indented with
spaces or tabs.

Markdown offers two styles of headers: *Setext* and *atx*.
Setext-style headers for `<h1>` and `<h2>` are created by
"underlining" with equal signs (`=`) and hyphens (`-`), respectively.
To create an atx-style header, you put 1-6 hash marks (`#`) at the
beginning of the line -- the number of hashes equals the resulting
HTML header level.

Blockquotes are indicated using email-style '`>`' angle brackets.

Markdown:

    A First Level Header
    ====================
    
    A Second Level Header
    ---------------------

    Now is the time for all good men to come to
    the aid of their country. This is just a
    regular paragraph.

    The quick brown fox jumped over the lazy
    dog's back.
    
    ### Header 3

    > This is a blockquote.
    > 
    > This is the second paragraph in the blockquote.
    >
    > ## This is an H2 in a blockquote


Output:

    <h1>A First Level Header</h1>
    
    <h2>A Second Level Header</h2>
    
    <p>Now is the time for all good men to come to
    the aid of their country. This is just a
    regular paragraph.</p>
    
    <p>The quick brown fox jumped over the lazy
    dog's back.</p>
    
    <h3>Header 3</h3>
    
    <blockquote>
        <p>This is a blockquote.</p>
        
        <p>This is the second paragraph in the blockquote.</p>
        
        <h2>This is an H2 in a blockquote</h2>
    </blockquote>



### Phrase Emphasis ###

Markdown uses asterisks and underscores to indicate spans of emphasis.

Markdown:

    Some of these words *are emphasized*.
    Some of these words _are emphasized also_.
    
    Use two asterisks for **strong emphasis**.
    Or, if you prefer, __use two underscores instead__.

Output:

    <p>Some of these words <em>are emphasized</em>.
    Some of these words <em>are emphasized also</em>.</p>
    
    <p>Use two asterisks for <strong>strong emphasis</strong>.
    Or, if you prefer, <strong>use two underscores instead</strong>.</p>
   


## Lists ##

Unordered (bulleted) lists use asterisks, pluses, and hyphens (`*`,
`+`, and `-`) as list markers. These three markers are
interchangable; this:

    *   Candy.
    *   Gum.
    *   Booze.

this:

    +   Candy.
    +   Gum.
    +   Booze.

and this:

    -   Candy.
    -   Gum.
    -   Booze.

all produce the same output:

    <ul>
    <li>Candy.</li>
    <li>Gum.</li>
    <li>Booze.</li>
    </ul>

Ordered (numbered) lists use regular numbers, followed by periods, as
list markers:

    1.  Red
    2.  Green
    3.  Blue

Output:

    <ol>
    <li>Red</li>
    <li>Green</li>
    <li>Blue</li>
    </ol>

If you put blank lines between items, you'll get `<p>` tags for the
list item text. You can create multi-paragraph list items by indenting
the paragraphs by 4 spaces or 1 tab:

    *   A list item.
    
        With multiple paragraphs.

    *   Another item in the list.

Output:

    <ul>
    <li><p>A list item.</p>
    <p>With multiple paragraphs.</p></li>
    <li><p>Another item in the list.</p></li>
    </ul>
    


### Links ###

Markdown supports two styles for creating links: *inline* and
*reference*. With both styles, you use square brackets to delimit the
text you want to turn into a link.

Inline-style links use parentheses immediately after the link text.
For example:

    This is an [example link](http://example.com/).

Output:

    <p>This is an <a href="http://example.com/">
    example link</a>.</p>

Optionally, you may include a title attribute in the parentheses:

    This is an [example link](http://example.com/ "With a Title").

Output:

    <p>This is an <a href="http://example.com/" title="With a Title">
    example link</a>.</p>

Reference-style links allow you to refer to your links by names, which
you define elsewhere in your document:

    I get 10 times more traffic from [Google][1] than from
    [Yahoo][2] or [MSN][3].

    [1]: http://google.com/        "Google"
    [2]: http://search.yahoo.com/  "Yahoo Search"
    [3]: http://search.msn.com/    "MSN Search"

Output:

    <p>I get 10 times more traffic from <a href="http://google.com/"
    title="Google">Google</a> than from <a href="http://search.yahoo.com/"
    title="Yahoo Search">Yahoo</a> or <a href="http://search.msn.com/"
    title="MSN Search">MSN</a>.</p>

The title attribute is optional. Link names may contain letters,
numbers and spaces, but are *not* case sensitive:

    I start my morning with a cup of coffee and
    [The New York Times][NY Times].

    [ny times]: http://www.nytimes.com/

Output:

    <p>I start my morning with a cup of coffee and
    <a href="http://www.nytimes.com/">The New York Times</a>.</p>


### Images ###

Image syntax is very much like link syntax.

Inline (titles are optional):

    ![alt text](/path/to/img.jpg "Title")

Reference-style:

    ![alt text][id]

    [id]: /path/to/img.jpg "Title"

Both of the above examples produce the same output:

    <img src="/path/to/img.jpg" alt="alt text" title="Title" />



### Code ###

In a regular paragraph, you can create code span by wrapping text in
backtick quotes. Any ampersands (`&`) and angle brackets (`<` or
`>`) will automatically be translated into HTML entities. This makes
it easy to use Markdown to write about HTML example code:

    I strongly recommend against using any `<blink>` tags.

    I wish SmartyPants used named entities like `&mdash;`
    instead of decimal-encoded entites like `&#8212;`.

Output:

    <p>I strongly recommend against using any
    <code>&lt;blink&gt;</code> tags.</p>
    
    <p>I wish SmartyPants used named entities like
    <code>&amp;mdash;</code> instead of decimal-encoded
    entites like <code>&amp;#8212;</code>.</p>


To specify an entire block of pre-formatted code, indent every line of
the block by 4 spaces or 1 tab. Just like with code spans, `&`, `<`,
and `>` characters will be escaped automatically.

Markdown:

    If you want your page to validate under XHTML 1.0 Strict,
    you've got to put paragraph tags in your blockquotes:

        <blockquote>
            <p>For example.</p>
        </blockquote>

Output:

    <p>If you want your page to validate under XHTML 1.0 Strict,
    you've got to put paragraph tags in your blockquotes:</p>
    
    <pre><code>&lt;blockquote&gt;
        &lt;p&gt;For example.&lt;/p&gt;
    &lt;/blockquote&gt;
    </code></pre>


PGP key/sig: https://keybase.io/russellbrandom/


<p>غش بناء الجملة:
تأكيد العبارة
<em>italic</em>   <strong>bold</strong>
<em>italic</em>   <strong>bold</strong>
الروابط
في النسق:</p>

<p>An <a href="http://url.com/" title="Title">example</a>
تسميات النمط المرجعي (العناوين اختيارية):</p>

<p>An <a href="/url/to/img.jpg" title="Title">example</a>. Then, anywhere
else in the doc, define the link:</p>

<p>الصور
مضمنة (العناوين اختيارية):</p>

<p><img src="/path/img.jpg" alt="alt text" title="Title" />
نمط المرجع:</p>

<p><img src="/url/to/img.jpg" alt="alt text" title="Title" /></p>

<p>الرؤوس
نمط Setext:</p>

<h1>Header 1</h1>

<h2>Header 2</h2>

<p>atx-style (إغلاق # اختيارية):</p>

<h1>Header 1</h1>

<h2>Header 2</h2>

<h6>Header 6</h6>

<p>القوائم
مرتبة ، بدون فقرات:</p>

<p><ol>
<li>Foo</li>
<li><p>Bar
بدون ترتيب ، مع فقرات:</p></li>
<li><p>A list item.</p></p>

<p>With multiple paragraphs.</p>

<p></li>
<li><p>Bar
يمكنك تداخلهم:</p></li>
<li><p>Abacus</p></p>

<ul><li>answer</li></ul>

<p></li>
<li>Bubbles</p>

<ol><li>bunk</li>
<li>bupkis
<ul><li>BELITTLER</li></ul></li>
<li>burper</li></ol>

<p></li>
<li>Cunning
كتلة الاقتباس</p>

<blockquote>
  <p>Email-style angle brackets
are used for blockquotes.</li>
</ol></p>

<blockquote>
  <p>And, they can be nested.</p>
</blockquote>

<h4>Headers in blockquotes</h4>

<ul>
<li>You can quote a list.</li>
<li>Etc.
يمتد كود
<code>&lt;code&gt;</code> spans are delimited
by backticks.</li>
</ul>
</blockquote>

<p>You can include literal backticks
like <code>`this`</code>.
كتل التعليمات البرمجية المنسقة مسبقًا
مسافة بادئة لكل سطر من كتلة التعليمات البرمجية بمقدار 4 مسافات على الأقل أو علامة تبويب واحدة.</p>

<p>This is a normal paragraph.</p>

<pre><code>This is a preformatted
code block.
</code></pre>

<p>القواعد الأفقية
ثلاث شرطات أو علامات نجمية أو أكثر:</p>

<hr />

<hr />

<hr />

<p>فواصل الأسطر اليدوية
قم بإنهاء سطر بمسافتين أو أكثر:</p>

<p>Roses are red, <br />
Violets are blue.
مصدر Markdown:</p>


Preview:

MainBasicsSyntaxLicenseDingus Syntax Cheatsheet: Phrase Emphasis italic bold italic bold Links Inline:

An example Reference-style labels (titles are optional):

An example. Then, anywhere else in the doc, define the link:

Images Inline (titles are optional):

alt text Reference-style:

alt text

Headers Setext-style:

Header 1
Header 2
atx-style (closing #'s are optional):

Header 1
Header 2
Header 6
Lists Ordered, without paragraphs:

Foo
Bar Unordered, with paragraphs:

A list item.

With multiple paragraphs.

Bar You can nest them:

Abacus

answer
Bubbles
bunk
bupkis
BELITTLER
burper
Cunning Blockquotes
Email-style angle brackets are used for blockquotes.

And, they can be nested.

Headers in blockquotes
You can quote a list.
Etc. Code Spans <code> spans are delimited by backticks.
You can include literal backticks like `this`. Preformatted Code Blocks Indent every line of a code block by at least 4 spaces or 1 tab.

This is a normal paragraph.

This is a preformatted
code block.
Horizontal Rules Three or more dashes or asterisks:


<p>MainBasicsSyntaxLicenseDingus
Syntax Cheatsheet:
Phrase Emphasis
<em>italic</em>   <strong>bold</strong>
<em>italic</em>   <strong>bold</strong>
Links
Inline:</p>

<p>An <a href="http://url.com/" title="Title">example</a>
Reference-style labels (titles are optional):</p>

<p>An <a href="/url/to/img.jpg" title="Title">example</a>. Then, anywhere
else in the doc, define the link:</p>

<p>Images
Inline (titles are optional):</p>

<p><img src="/path/img.jpg" alt="alt text" title="Title" />
Reference-style:</p>

<p><img src="/url/to/img.jpg" alt="alt text" title="Title" /></p>

<p>Headers
Setext-style:</p>

<h1>Header 1</h1>

<h2>Header 2</h2>

<p>atx-style (closing #'s are optional):</p>

<h1>Header 1</h1>

<h2>Header 2</h2>

<h6>Header 6</h6>

<p>Lists
Ordered, without paragraphs:</p>

<p><ol>
<li>Foo</li>
<li><p>Bar
Unordered, with paragraphs:</p></li>
<li><p>A list item.</p></p>

<p>With multiple paragraphs.</p>

<p></li>
<li><p>Bar
You can nest them:</p></li>
<li><p>Abacus</p></p>

<ul><li>answer</li></ul>

<p></li>
<li>Bubbles</p>

<ol><li>bunk</li>
<li>bupkis
<ul><li>BELITTLER</li></ul></li>
<li>burper</li></ol>

<p></li>
<li>Cunning
Blockquotes</p>

<blockquote>
  <p>Email-style angle brackets
are used for blockquotes.</li>
</ol></p>

<blockquote>
  <p>And, they can be nested.</p>
</blockquote>

<h4>Headers in blockquotes</h4>

<ul>
<li>You can quote a list.</li>
<li>Etc.
Code Spans
<code>&lt;code&gt;</code> spans are delimited
by backticks.</li>
</ul>
</blockquote>

<p>You can include literal backticks
like <code>`this`</code>.
Preformatted Code Blocks
Indent every line of a code block by at least 4 spaces or 1 tab.</p>

<p>This is a normal paragraph.</p>

<pre><code>This is a preformatted
code block.
</code></pre>

<p>Horizontal Rules
Three or more dashes or asterisks:</p>

<hr />

<hr />

<hr />

<p>Manual Line Breaks
End a line with two or more spaces:</p>

<p>Roses are red, <br />
Violets are blue.
Markdown Source:</p>


"This XML file does not appear to have any style information associated with it. The document tree is shown below.
<rss xmlns:content="http://purl.org/rss/1.0/modules/content/" xmlns:itunes="http://www.itunes.com/dtds/podcast-1.0.dtd" xmlns:media="http://www.rssboard.org/media-rss" version="2.0">
<channel>
<title>The Talk Show With John Gruber</title>
<link>https://daringfireball.net/thetalkshow</link>
<description>The director’s commentary track for Daring Fireball.</description>
<docs>http://blogs.law.harvard.edu/tech/rss</docs>
<language>en</language>
<pubDate>Sat, 18 Sep 2021 14:06:16 EDT</pubDate>
<lastBuildDate>Sat, 18 Sep 2021 14:06:16 EDT</lastBuildDate>
<itunes:new-feed-url>https://daringfireball.net/thetalkshow/rss</itunes:new-feed-url>
<itunes:author>Daring Fireball / John Gruber</itunes:author>
<itunes:summary>The director’s commentary track for Daring Fireball.</itunes:summary>
<itunes:keywords>john gruber, daring fireball, apple, mac, iphone, ipad, tech</itunes:keywords>
<itunes:image href="https://daringfireball.net/thetalkshow/graphics/df-the-talk-show-album-art.png"/>
<itunes:explicit>no</itunes:explicit>
<itunes:owner>
<itunes:name>John Gruber</itunes:name>
<itunes:email>comments@daringfireball.net</itunes:email>
</itunes:owner>
<itunes:category text="Technology"> </itunes:category>
<!--  Latest  -->
<item>
<title>322: ‘It Was More Arial Than Helvetica’, With Rene Ritchie</title>
<link>https://daringfireball.net/thetalkshow/2021/09/18/ep-322</link>
<guid>https://daringfireball.net/thetalkshow/2021/09/18/ep-322</guid>
<pubDate>Sat, 18 Sep 2021 14:06:16 EDT</pubDate>
<enclosure url="https://traffic.libsyn.com/secure/daringfireball/thetalkshow-322-rene-ritchie.mp3" length="59910341" type="audio/mpeg"/>
<itunes:duration>02:04:29</itunes:duration>
<itunes:explicit>no</itunes:explicit>
<itunes:author>Daring Fireball / John Gruber</itunes:author>
<description>Rene Ritchie returns to the show for a recap of this week’s “California Streaming” Apple Event: the iPhones 13, Apple Watch Series 7, and new iPads. Also, last week’s decision in the Apple v. Epic lawsuit.</description>
<itunes:image href="https://daringfireball.net/thetalkshow/graphics/df-the-talk-show-album-art.png"/>
<content:encoded>
<![CDATA[ <p>Rene Ritchie returns to the show for a recap of this week’s “California Streaming” Apple Event: the iPhones 13, Apple Watch Series 7, and new iPads. Also, last week’s decision in the Apple v. Epic lawsuit.</p> <p>Sponsored by:</p> <ul> <li><a href="https://squarespace.com/talkshow">Squarespace</a>: Make your next move. Use code <strong>talkshow</strong> for 10% off your first order.</li> <li><a href="https://hellofresh.com/talkshow14">Hello Fresh</a>: America’s #1 meal kit.</li> <li><a href="https://awaytravel.com/talkshow">Away</a>: Designed to last for life.</li> </ul> <p>Links:</p> <ul> <li><a href="https://www.apple.com/apple-events/september-2021/">Apple’s event page for “California Streaming”</a>.</li> <li><a href="https://daringfireball.net/2021/09/california_streaming_thoughts_and_observations">Yours truly’s thoughts and observations</a>.</li> <li><a href="https://daringfireball.net/linked/2021/09/10/judgment-in-epic-v-apple">Judge Yvonne Gonzalez Rogers’s decision in the Apple v. Epic case</a>.</li> <li><a href="https://twitter.com/StephenWarwick9/status/1436421603206778883">Stephen Warwick’s humorous summary of the decision</a>.</li> </ul> <p><em>This episode of The Talk Show was edited by Caleb Sexton.</em></p> ]]>
</content:encoded>
</item>
<!--  /Latest  -->
<item>
<title>321: ‘Just a Standard Bird’, With MG Siegler</title>
<link>https://daringfireball.net/thetalkshow/2021/08/31/ep-321</link>
<guid>https://daringfireball.net/thetalkshow/2021/08/31/ep-321</guid>
<pubDate>Tue, 31 Aug 2021 23:56:00 EDT</pubDate>
<enclosure url="https://traffic.libsyn.com/secure/daringfireball/thetalkshow-321-mg-siegler.mp3" length="57404073" type="audio/mpeg"/>
<itunes:duration>01:57:58</itunes:duration>
<itunes:explicit>no</itunes:explicit>
<itunes:author>Daring Fireball / John Gruber</itunes:author>
<description>MG Siegler returns to the show to talk about last week’s surprise announcement from Apple settling a class action lawsuit filed on behalf of U.S. App Store developers, and the various reactions to it. Also, a bit on App Store payment processing, and some speculation on who might succeed Tim Cook.</description>
<itunes:image href="https://daringfireball.net/thetalkshow/graphics/df-the-talk-show-album-art.png"/>
<content:encoded>
<![CDATA[ <p>MG Siegler returns to the show to talk about last week’s surprise announcement from Apple settling a class action lawsuit filed on behalf of U.S. App Store developers, and the various reactions to it. Also, a bit on App Store payment processing, and some speculation on who might succeed Tim Cook.</p> <p>Sponsored by:</p> <ul> <li><a href="https://squarespace.com/talkshow">Squarespace</a>: Make your next move. Use code <strong>talkshow</strong> for 10% off your first order.</li> <li><a href="https://mackweldon.com/talkshow">Mack Weldon</a>: Reinventing men’s basics with smart design, premium fabrics, and simple shopping. Get 20% off your first order with code <strong>talkshow</strong>.</li> <li><a href="https://linode.com/thetalkshow">Linode</a>: Instantly deploy and manage an SSD server in the Linode Cloud. New accounts get a $100 credit.</li> <li><a href="https://madeincookware.com/thetalkshow">Made In</a>: Better cookware for better meals. Get 15% off your first order with code <strong>THETALKSHOW</strong>.</li> </ul> <p>Links:</p> <ul> <li><a href="https://www.apple.com/newsroom/2021/08/apple-us-developers-agree-to-app-store-updates/">Apple’s masterful press release that got them just the headlines they were hoping to get</a>.</li> <li><a href="https://www.techmeme.com/210826/p38#a210826p38">Techmeme’s roundup of Big Press headlines regarding Apple’s settlement proposal for the class action lawsuit regarding the App Store in the U.S</a>.</li> <li><a href="https://www.bloomberg.com/news/articles/2021-08-27/apple-settlement-lets-app-developers-advertise-outside-payments">Bloomberg got it right: “Apple Settles With App Developers Without Making Major Concessions”</a>.</li> <li><a href="https://twitter.com/rjonesy/status/1431080067942207488">Ryan Jones’s excellent Twitter thread that accurately depicts the actual nature of Apple’s settlement proposal</a>.</li> <li><a href="https://www.nytimes.com/2021/08/27/technology/apple-app-settlement-explained.html">Jack Nicas’s column for the NYT: “Why Apple Won Its Legal Settlement With Developers”</a>.</li> <li><a href="https://500ish.com/thank-you-apple-may-we-have-another-115b91ad1773">MG on Apple’s press release: “Thank You, Apple! May We Have Another?”</a>.</li> <li><a href="https://500ish.com/apple-accentuates-the-positive-837b6673ea56">And MG’s follow-up, “Apple Accentuates the Positive”</a>.</li> <li><a href="https://www.apple.com/newsroom/2021/08/apple-introduces-the-news-partner-program/">Apple’s earlier-on-Thursday announcement regarding the News Partner Program</a>.</li> <li><a href="https://daringfireball.net/2021/06/app_store_the_schiller_cut">Phil Schiller’s 2011 memo asking “Do we think our 70/30 split will last forever?”</a>.</li> <li><a href="https://www.bloomberg.com/news/newsletters/2021-08-29/who-will-replace-tim-cook-as-the-next-ceo-of-apple-aapl-ksxiq29z">Mark Gurman’s latest column, speculating on who might succeed Tim Cook as CEO</a>.</li> <li><a href="https://en.wikipedia.org/wiki/Peter_principle">The Peter Principle</a> — “a concept in management developed by Laurence J. Peter, which observes that people in a hierarchy tend to rise to their ‘maximum level of incompetence’”. (I blew it and said “<a href="https://en.wikipedia.org/wiki/Pareto_principle">Pareto Principle</a>” on air, which is an entirely different thing, but also interesting.)</li> <li><a href="https://www.youtube.com/watch?v=9sIiajEEETw">Randy Johnson hits a bird with a pitch during a 2001 preseason MLB game</a>.</li> </ul> <p><em>This episode of The Talk Show was edited by Caleb Sexton.</em></p> ]]>
</content:encoded>
</item>
<item>
<title>320: ‘Paper Floor Mats’, With Christina Warren</title>
<link>https://daringfireball.net/thetalkshow/2021/08/23/ep-320</link>
<guid>https://daringfireball.net/thetalkshow/2021/08/23/ep-320</guid>
<pubDate>Mon, 23 Aug 2021 15:25:03 EDT</pubDate>
<enclosure url="https://traffic.libsyn.com/secure/daringfireball/thetalkshow-320-christina-warren.mp3" length="61850204" type="audio/mpeg"/>
<itunes:duration>02:08:32</itunes:duration>
<itunes:explicit>no</itunes:explicit>
<itunes:author>Daring Fireball / John Gruber</itunes:author>
<description>Christina Warren returns to the show to discuss Apple’s controversial child safety initiatives, the tumultuous summer of Safari 15 beta UI designs, and a bit more on MagSafe battery packs.</description>
<itunes:image href="https://daringfireball.net/thetalkshow/graphics/df-the-talk-show-album-art.png"/>
<content:encoded>
<![CDATA[ <p>Christina Warren returns to the show to discuss Apple’s controversial child safety initiatives, the tumultuous summer of Safari 15 beta UI designs, and a bit more on MagSafe battery packs.</p> <p>Sponsored by:</p> <ul> <li><a href="https://squarespace.com/talkshow">Squarespace</a>: Make your next move. Use code <strong>talkshow</strong> for 10% off your first order.</li> <li><a href="https://memberful.com/talkshow">Memberful</a>: Monetize your passion with membership.</li> <li><a href="https://awaytravel.com/talkshow">Away</a>: Because this season, everyone wants to get Away.</li> <li><a href="https://hover.com/talkshow">Hover</a>: Find a domain name for your passion. Get 10% off your first purchase.</li> </ul> <p>Links:</p> <ul> <li><a href="https://www.monotype.com/fonts/helvetica-now-variable">Monotype Helvetica Now Variable</a>.</li> <li><a href="https://www.youtube.com/watch?v=cVT-8mBuGok">Quinn Nelson's skewering of Apple's MagSafe Battery Pack</a>.</li> <li><a href="https://us.anker.com/collections/portable-power/products/a1619">Anker's superior $55 MagSafe-compatible battery pack</a>.</li> <li><a href="https://daringfireball.net/2021/08/apple_child_safety_initiatives_slippery_slope">Yours truly on Apple's child safety initiatives</a>.</li> </ul> <p><em>This episode of The Talk Show was edited by Caleb Sexton.</em></p> ]]>
</content:encoded>
</item>
<item>
<title>319: ‘You Called Him Pixel Mature’, With John Moltz</title>
<link>https://daringfireball.net/thetalkshow/2021/07/30/ep-319</link>
<guid>https://daringfireball.net/thetalkshow/2021/07/30/ep-319</guid>
<pubDate>Fri, 30 Jul 2021 16:41:24 EDT</pubDate>
<enclosure url="https://traffic.libsyn.com/secure/daringfireball/thetalkshow-319-john-moltz.mp3" length="51413397" type="audio/mpeg"/>
<itunes:duration>01:46:33</itunes:duration>
<itunes:explicit>no</itunes:explicit>
<itunes:author>Daring Fireball / John Gruber</itunes:author>
<description>Special guest: John Moltz. Special topics: Playdate preorders, MagSafe battery packs, iPad keyboard covers, Facebook and NSO Group, Safari 15 betas, and “Loki”.</description>
<itunes:image href="https://daringfireball.net/thetalkshow/graphics/df-the-talk-show-album-art.png"/>
<content:encoded>
<![CDATA[ <p>Special guest: John Moltz. Special topics: Playdate preorders, MagSafe battery packs, iPad keyboard covers, Facebook and NSO Group, Safari 15 betas, and <em>Loki</em>.</p> <p>Sponsored by:</p> <ul> <li><a href="https://linkedin.com/talk">LinkedIn Jobs</a>: Find and hire the right person. Your first job post is free.</li> <li><a href="https://awaytravel.com/talkshow">Away</a>: Because this season, everyone wants to get Away.</li> <li><a href="https://squarespace.com/talkshow">Squarespace</a>: Everything you need to grow online. Use code <strong>talkshow</strong> for 10% off your first order.</li> <li><a href="https://linode.com/thetalkshow">Linode</a>: Instantly deploy and manage an SSD server in the Linode Cloud. New accounts get a $100 credit.</li> <li><a href="https://mackweldon.com/talkshow">Mack Weldon</a>: Reinventing men’s basics with smart design, premium fabrics, and simple shopping. Get 20% off your first order with code <strong>talkshow</strong>.</li> </ul> <p>Links:</p> <ul> <li><a href="https://www.apple.com/newsroom/2021/08/apple-us-developers-agree-to-app-store-updates/">Apple’s masterful press release that got them just the headlines they were hoping to get</a>.</li> <li><a href="https://www.techmeme.com/210826/p38#a210826p38">Techmeme’s roundup of Big Press headlines regarding Apple’s settlement proposal for the class action lawsuit regarding the App Store in the U.S</a>.</li> <li><a href="https://www.bloomberg.com/news/articles/2021-08-27/apple-settlement-lets-app-developers-advertise-outside-payments">Bloomberg got it right: “Apple Settles With App Developers Without Making Major Concessions”</a>.</li> <li><a href="https://twitter.com/rjonesy/status/1431080067942207488">Ryan Jones’s excellent Twitter thread that accurately depicts the actual nature of Apple’s settlement proposal</a>.</li> <li><a href="https://www.nytimes.com/2021/08/27/technology/apple-app-settlement-explained.html">Jack Nicas’s column for the NYT: “Why Apple Won Its Legal Settlement With Developers”</a>.</li> <li><a href="https://500ish.com/thank-you-apple-may-we-have-another-115b91ad1773">MG on Apple’s press release: “Thank You, Apple! May We Have Another?”</a>.</li> <li><a href="https://500ish.com/apple-accentuates-the-positive-837b6673ea56">And MG’s follow-up, “Apple Accentuates the Positive”</a>.</li> <li><a href="https://www.apple.com/newsroom/2021/08/apple-introduces-the-news-partner-program/">Apple’s earlier-on-Thursday announcement regarding the News Partner Program</a>.</li> <li><a href="https://daringfireball.net/2021/06/app_store_the_schiller_cut">Phil Schiller’s 2011 memo asking “Do we think our 70/30 split will last forever?”</a>.</li> <li><a href="https://www.bloomberg.com/news/newsletters/2021-08-29/who-will-replace-tim-cook-as-the-next-ceo-of-apple-aapl-ksxiq29z">Mark Gurman’s latest column, speculating on who might succeed Tim Cook as CEO</a>.</li> <li><a href="https://en.wikipedia.org/wiki/Peter_principle">The Peter Principle</a> — “a concept in management developed by Laurence J. Peter, which observes that people in a hierarchy tend to rise to their ‘maximum level of incompetence’”. (I blew it and said “<a href="https://en.wikipedia.org/wiki/Pareto_principle">Pareto Principle</a>” on air, which is an entirely different thing, but also interesting.)</li> <li>Another post-show correction: there <em>is</em> one MLB team <a href="https://daringfireball.net/misc/2021/08/the-oriole-bird.jpeg">with a friendly bird mascot</a>. (I mistakenly thought they had been relegated to AAA, and regret the error.)</li> <li><a href="https://www.youtube.com/watch?v=9sIiajEEETw">Randy Johnson hits a bird with a pitch during a 2001 preseason MLB game</a>.</li> </ul> <p><em>This episode of The Talk Show was edited by Caleb Sexton.</em></p> ]]>
</content:encoded>
</item>
<item>
<title>318: ‘Holes in the Blast Door’, With Matthew Panzarino</title>
<link>https://daringfireball.net/thetalkshow/2021/07/21/ep-318</link>
<guid>https://daringfireball.net/thetalkshow/2021/07/21/ep-318</guid>
<pubDate>Thu, 22 Jul 2021 00:38:33 EDT</pubDate>
<enclosure url="https://traffic.libsyn.com/secure/daringfireball/thetalkshow-318-matthew-panzarino.mp3" length="60975081" type="audio/mpeg"/>
<itunes:duration>02:06:29</itunes:duration>
<itunes:explicit>no</itunes:explicit>
<itunes:author>Daring Fireball / John Gruber</itunes:author>
<description>Matthew Panzarino returns to the show. Topics include: Apple’s new MagSafe Battery Pack, the Amnesty-International-Led exposé of NSO Group’s state-sponsored phone hacking, Safari 15’s controversial new UI and Apple’s response, and a look back at year one of Apple silicon for Macs. Also: pizza.</description>
<itunes:image href="https://daringfireball.net/thetalkshow/graphics/df-the-talk-show-album-art.png"/>
<content:encoded>
<![CDATA[ <p>Matthew Panzarino returns to the show. Topics include: Apple’s new MagSafe Battery Pack, the Amnesty-International-Led exposé of NSO Group’s state-sponsored phone hacking, Safari 15’s controversial new UI and Apple’s response, and a look back at year one of Apple silicon for Macs. Also: pizza.</p> <p>Sponsored by:</p> <ul> <li><a href="https://hellofresh.com/talkshow14">Hello Fresh</a>: America’s #1 Meal Kit</li> <li><a href="https://squarespace.com/talkshow">Squarespace</a>: Everything you need to grow online. Use code <strong>talkshow</strong> for 10% off your first order.</li> <li><a href="https://memberful.com/talkshow">Memberful</a>: Monetize your passion with membership.</li> <li><a href="https://linode.com/thetalkshow">Linode</a>: Instantly deploy and manage an SSD server in the Linode Cloud. New accounts get a $100 credit.</li> </ul> <p>Links:</p> <ul> <li>Battery Packs: <ul><li><a href="https://store.apple.com/xc/product/MJWY3AM/A">Apple’s $99 MagSafe Battery Pack</a></li> <li><a href="https://us.anker.com/products/a1619">Anker’s $46 PowerCore Magnetic 5K MagSafe-compatible battery pack</a></l


This XML file does not appear to have any style information associated with it. The document tree is shown below.
<feed xmlns="http://www.w3.org/2005/Atom">
<title>Daring Fireball</title>
<subtitle>By John Gruber</subtitle>
<link rel="alternate" type="text/html" href="https://daringfireball.net/"/>
<link rel="self" type="application/atom+xml" href="https://daringfireball.net/feeds/main"/>
<id>https://daringfireball.net/feeds/main</id>
<updated>2021-09-27T23:28:04Z</updated>
<rights>Copyright © 2021, John Gruber</rights>
<entry>
<link rel="alternate" type="text/html" href="https://quill.chat/"/>
<link rel="shorturl" href="http://df4.us/top"/>
<link rel="related" type="text/html" href="https://daringfireball.net/feeds/sponsors/2021/09/quill_messaging_to_make_your_t_1"/>
<id>tag:daringfireball.net,2021:/feeds/sponsors//11.38473</id>
<author>
<name>Daring Fireball Department of Commerce</name>
</author>
<published>2021-09-27T18:31:53-05:00</published>
<updated>2021-09-27T18:31:53-05:00</updated>
<content type="html" xml:base="https://daringfireball.net/feeds/sponsors/" xml:lang="en">
<![CDATA[ <p>We love messaging (and most of us grew up using IRC.) It’s our favorite way of collaborating, but not if it’s overwhelming and disorganized. We grew exhausted having to skim thousands of messages every day to keep up, so we built something better. A more deliberate way to chat.</p> <div> <a title="Permanent link to ‘Quill — Messaging to Make Your Team Better’" href="https://daringfireball.net/feeds/sponsors/2021/09/quill_messaging_to_make_your_t_1">&nbsp;★&nbsp;</a> </div> ]]>
</content>
<title>[Sponsor] Quill — Messaging to Make Your Team Better</title>
</entry>
<entry>
<link rel="alternate" type="text/html" href="https://daringfireball.net/2021/09/why_still_lightning"/>
<link rel="shorturl" href="http://df4.us/too"/>
<id>tag:daringfireball.net,2021://1.38472</id>
<published>2021-09-27T18:27:45Z</published>
<updated>2021-09-27T23:28:04Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<summary type="text">My theory is that Apple carefully weighs the pros and cons for each port on each device it makes, and chooses the one that it thinks makes for the best product for the most people.</summary>
<content type="html" xml:base="https://daringfireball.net/" xml:lang="en">
<![CDATA[ <p>Chaim Gartenberg, writing for The Verge, “<a href="https://www.theverge.com/2021/9/24/22690338/apple-iphone-lightning-ports-convenience-control-usb-c-eu-wireless-charging-mfi-magsafe">The Lightning Port Isn’t About Convenience; It’s About Control</a>”:</p> <blockquote> <p>Notably absent from Apple’s argument, though, is the fact that cutting out a Lightning port on an iPhone wouldn’t just create more e-waste (if you buy Apple’s logic) or inconvenience its customers. It also means that Apple would lose out on the revenue it makes from every Lightning cable and accessory that works with the iPhone, Apple-made or not — along with the control it has over what kinds of hardware does (or doesn’t) get to exist for the iPhone and which companies get to make them.</p> <p>Apple’s <a href="https://mfi.apple.com/">MFi program</a> means that if you want to plug anything into an iPhone, be it charger or adapter or accessory, you have to go through Apple. And Apple takes a cut of every one of those devices, too.</p> </blockquote> <p>Gartenberg summarizes a commonly-held theory here: that Apple is sticking with its proprietary Lightning port on iPhones because they profit from MFi peripherals. That it’s a money grab.</p> <p>I don’t think this is the case at all. Apple is happy to keep the money it earns from MFi, of course. And they’re glad to have control over all iPhone peripherals. But I don’t think there’s serious money in that. It’s loose-change-under-the-couch-cushion revenue by Apple’s astonishingly high standards. How many normal people do you know who ever buy <em>anything</em> that plugs into a Lightning port other than a USB cable? And Apple doesn’t make more money selling their own (admittedly overpriced) Lightning cables to iPhone owners than they do selling their own (also overpriced) USB-C cables to iPad Pro and MacBook owners.</p> <p>My theory is that Apple carefully weighs the pros and cons for each port on each device it makes, and chooses the technologies for those ports that it thinks makes for the best product for the most people. “<em>What makes sense for the goals of this product that we will ship in three years? And then the subsequent models for the years after that?</em>” Those are the questions Apple product designers ask.</p> <p>The sub-head on Gartenberg’s piece is “The iPhone doesn’t have USB-C for a reason”. Putting that in the singular does not do justice to the complexity of such decisions. There are numerous reasons that the iPhones 13 still use Lightning — <em>and</em> there are numerous reasons why switching to USB-C would make sense. The pro-USB-C crowd, to me, often comes across as ideological. I’m not accusing Gartenberg of this — though it is his piece with the sub-head claiming there’s “a” singular reason — but many iPhones-should-definitely-use-USB-C proponents argue as though there are no good reasons for the iPhone to continue using Lightning. That’s nonsense.</p> <p>To be clear, I’m neither pro-Lightning nor pro-USB-C. I see the trade-offs. If the iPhones 13 had switched to USB-C, I wouldn’t have complained. But I didn’t complain about them not switching, either. You’ll note that in none of my reviews of iPad models that have switched from Lightning to USB-C in recent years have I complained about the switch. Apple, to my eyes, has been managing this well. But, if the iPhones 13 <em>had</em> switched to USB-C, you know who <em>would</em> have complained? <em>Hundreds of millions of existing iPhone users</em> who have no interest in replacing the Lightning cables and docks they already own.</p> <p>When Lightning replaced the old 30-pin iPod connector, starting with the iPhone 5 in 2012, many — I’d say <em>most</em> — existing iPhone users were not happy about it. Many were downright angry. It didn’t matter that the old 30-pin adapter was, compared to Lightning, hideously ungainly, far too large, and technically outdated. (Also, I believe the 30-pin port was impossible or nearly-impossible to make waterproof. The first waterproof models <a href="https://support.apple.com/kb/SP743?locale=en_US">were the iPhones 7 in 2016</a>.) People do not like buying new cables, no matter if they’re “better”. Now, I know what you, someone reading Daring Fireball, might be thinking — <em>I own dozens of USB-C cables already</em> — because you own other products, perhaps several from Apple itself, that do use USB-C. But that’s not true for most iPhone owners around the world. They have Lightning chargers in their kitchens, cars, purses, backpacks, and bedrooms. All things considered, they do not want to replace any of them, let alone all of them.</p> <p>In 15 generations of iPhones, Apple has changed the connector once. And that one time was a clear win in every single regard. Changing from Lightning to USB-C is not so clearly an upgrade at all. It’s a sidestep. Note too that when Apple first started changing iPads — <a href="https://techcrunch.com/2018/10/30/the-ipad-finally-moves-to-usb-c/">starting with the iPad Pro in late 2018</a> — from Lightning to USB-C, they didn’t say it was because USB-C is better, period, and certainly not solely for the reason that USB-C is “open”. They said it was to enable iPads Pro to do things that theretofore only PCs and Macs could do, like connecting to external displays. iPhones aren’t meant for that. Or at least aren’t meant for that <em>yet</em> — if ever they are, iPhone peripheral capabilities, including hardware ports, will change.</p> <p>If you’re on team “Lightning is nothing but a money grab”, you should explain why, for inductive (a.k.a. wireless) charging, iPhones have supported industry-standard Qi from day one. Or why iPads have been steadily moving from Lightning to USB-C. Or why Apple was the first laptop maker to go all-in on USB-C, literally <a href="https://www.macworld.com/article/225278/review-the-new-12-inch-macbook-is-a-laptop-without-an-ecosystem.html">making a laptop with no ports other than a single USB-C port</a> and a headphone jack.</p> <p>Speaking of headphone jacks, my theory is the same with those. Apple’s not “against” headphone jacks. They’ve begun steadily removing them from new products only when they deem doing so the best trade-off. The <a href="https://support.apple.com/kb/SP850">new iPad Mini</a> has no headphone jack; the <a href="https://support.apple.com/kb/SP849">new regular iPad</a> that debuted alongside it does. That’s not ideal, but it’s not incoherent. They are different products for different users with different needs and different priorities. These decisions require nuance. “<em>Apple’s just trying to force everyone to buy $160 AirPods</em>” is not a nuanced argument. Is it a consideration that removing the headphone jack from more products each year might steer more customers toward their first AirPods purchase? Sure. But it’s not like there aren’t other brands of wireless headphones.</p> <p>To say that there’s <em>a</em> reason that the iPhones 13 still use Lightning, any singular reason, is facile.</p> ]]>
</content>
<title>★ Why Does the iPhone Still Use Lightning?</title>
</entry>
<entry>
<title>Yours Truly on The HourTime Show</title>
<link rel="alternate" type="text/html" href="https://anchor.fm/the-hourtime-show/episodes/Why-Its-So-Hard-to-Buy-a-Rolex-Gruber-Guest-Appearance-e17tji8"/>
<link rel="shorturl" type="text/html" href="http://df4.us/ton"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/27/the-hourtime-show"/>
<id>tag:daringfireball.net,2021:/linked//6.38471</id>
<published>2021-09-27T17:25:03Z</published>
<updated>2021-09-27T17:25:03Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>I had the distinct pleasure of a guest appearance on this week’s episode of The HourTime Show, a watch nerd podcast from the gang at WristWatchReview — John Biggs, Victor Marks, and Nicholas De Leon. The topic: why it’s <a href="https://www.wristwatchreview.com/rolex-claims-the-supply-shortage-is-not-planned-unconvincingly/">so crazy hard</a> to buy a new Rolex.</p> <div> <a title="Permanent link to ‘Yours Truly on The HourTime Show’" href="https://daringfireball.net/linked/2021/09/27/the-hourtime-show">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Wil Shipley Joins Apple</title>
<link rel="alternate" type="text/html" href="https://twitter.com/wilshipley/status/1442528831689007112"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tom"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/27/shipley-apple"/>
<id>tag:daringfireball.net,2021:/linked//6.38470</id>
<published>2021-09-27T17:19:00Z</published>
<updated>2021-09-27T17:19:00Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>On the one hand, I did not see that coming. On the other hand is <a href="https://twitter.com/atomicbird/status/499576229734150144">this apt observation from Tom Harrington</a>:</p> <blockquote> <p>How to make technical contacts at Apple:</p> <ol> <li>Meet any developer who knows what they’re doing.</li> <li>Wait.</li> <li>They now work for Apple.</li> </ol> </blockquote> <div> <a title="Permanent link to ‘Wil Shipley Joins Apple’" href="https://daringfireball.net/linked/2021/09/27/shipley-apple">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>If Unlock With Apple Watch Isn’t Working on Your iPhone 13</title>
<link rel="alternate" type="text/html" href="https://support.apple.com/en-us/HT212828"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tol"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/27/apple-watch-unlock-iphone-13"/>
<id>tag:daringfireball.net,2021:/linked//6.38469</id>
<published>2021-09-27T14:43:23Z</published>
<updated>2021-09-27T14:44:44Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Apple support document acknowledges a problem a lot of iPhone 13 users are running into:</p> <blockquote> <p>Apple has identified an issue where <a href="https://support.apple.com/kb/HT212208">Unlock with Apple Watch</a> may not work with iPhone 13 devices. You might see “Unable to Communicate with Apple Watch” if you try to unlock your iPhone while wearing a face mask, or you might not be able to set up Unlock with Apple Watch.</p> <p>This issue will be fixed in an upcoming software update. Until the update is available, you can turn off Unlock with Apple Watch and use your passcode to unlock your iPhone 13.</p> </blockquote> <p>I haven’t seen this issue, but I sympathize with those of you who’ve been hit by it. “Unlock With Apple Watch” almost completely mitigates the annoyance of using an iPhone with Face ID while wearing a mask.</p> <div> <a title="Permanent link to ‘If Unlock With Apple Watch Isn’t Working on Your iPhone 13’" href="https://daringfireball.net/linked/2021/09/27/apple-watch-unlock-iphone-13">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Retool</title>
<link rel="alternate" type="text/html" href="https://retool.com/?utm_source=sponsor&utm_medium=newsletter&utm_campaign=daringfireball"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tok"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/26/retool"/>
<id>tag:daringfireball.net,2021:/linked//6.38468</id>
<published>2021-09-26T21:29:30Z</published>
<updated>2021-09-26T21:30:13Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>My thanks to Retool for sponsoring last week at DF. Retool is a new approach to programming for the modern web: they’ve unified the ease of visual programming with the power and flexibility of real code. Drag and drop a form together, and have it <code>POST</code> back to your API in minutes. Deploy instantly with access controls and audit logs. It’s akin to a HyperCard or Visual Basic for the modern web.</p> <p>Allbirds uses Retool to measure billboard efficacy. Amazon uses Retool to handle GDPR requests. You, too, can use it to build business-critical applications fast.</p> <p>Check out their demo video to see how easy it is to build something serious and useful — quickly and intuitively. It’s easy to explore on your own <em>and</em> they have <a href="https://docs.retool.com/docs">good docs</a> and guided videos. <a href="https://retool.com/?utm_source=sponsor&amp;utm_medium=newsletter&amp;utm_campaign=daringfireball">Start building for free today</a>.</p> <div> <a title="Permanent link to ‘Retool’" href="https://daringfireball.net/linked/2021/09/26/retool">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Arun Maini’s Battery Life Stress Test for the New iPhones 13</title>
<link rel="alternate" type="text/html" href="https://www.youtube.com/watch?v=IQQCoJiZj8w"/>
<link rel="shorturl" type="text/html" href="http://df4.us/toj"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/25/arun-maini-iphone-13-battery-stress-test"/>
<id>tag:daringfireball.net,2021:/linked//6.38467</id>
<published>2021-09-25T21:00:30Z</published>
<updated>2021-09-25T21:00:31Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>YouTuber Arun “Mrwhosetheboss” Maini’s full battery life drain test of the iPhone 13 Pro Max, iPhone 13 Pro, iPhone 13, iPhone 13 Mini, iPhone 12, iPhone 11, and iPhone SE. Interesting results that jibe with Apple’s claims about the improvements to battery life in the iPhones 13.</p> <p><a href="https://twitter.com/greengart/status/1441426882893914112">Via Avi Greengart</a>, who observes the most impressive result:</p> <blockquote> <p>It’s worth watching Arun’s whole video, but the iPhone 13 mini handily beats last year’s full-sized iPhone 12 on battery life, making it an easy recommendation for anyone with human-sized hands. The entire iPhone 13 line has genuinely good to extraordinary battery life.</p> </blockquote> <p>The iPhone 13 Mini has longer battery life than last year’s regular iPhone 12. That’s a game-changer for those who want the Mini size.</p> <div> <a title="Permanent link to ‘Arun Maini’s Battery Life Stress Test for the New iPhones 13’" href="https://daringfireball.net/linked/2021/09/25/arun-maini-iphone-13-battery-stress-test">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Try Safari 15 Before You Buy, With Safari Technology Preview</title>
<link rel="alternate" type="text/html" href="https://developer.apple.com/safari/technology-preview/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/toi"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/25/try-safari-15-tech-preview"/>
<id>tag:daringfireball.net,2021:/linked//6.38466</id>
<published>2021-09-25T20:23:01Z</published>
<updated>2021-09-25T20:23:02Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>MacOS 12 Monterey is not out yet — and, I hope, won’t ship until after a few more weeks of much-needed bug fixes — but Safari 15 for MacOS 11 Big Sur <a href="https://arstechnica.com/gadgets/2021/09/apple-rolls-major-safari-redesign-out-to-macs-ahead-of-monterey-release/">shipped last week</a>. I strongly recommend <em>not</em> upgrading, unless you’ve already tried the new tab design and like it, or at least feel ambivalent about it. Updates like this are why I always <a href="/misc/2021/09/software-update-auto-checkbox.png">turn off “Automatically keep my Mac up to date”</a> in System Preferences → Software Update.</p> <p>The sole reason I recommend not upgrading to Safari 15 is the new tab bar design. You can easily try it out for yourself, though, without upgrading to Safari 15 or installing the MacOS 12 betas. Safari Technology Preview is a <em>separate</em> version of Safari you can easily install next to regular Safari. Typically it’s used by web developers to test in-progress changes to WebKit, but right now it’s more useful as a way to preview the new Safari 15 tab design. It’s easy to install and easy to uninstall. You can even set it as your default web browser while testing in System Preferences: General.</p> <div> <a title="Permanent link to ‘Try Safari 15 Before You Buy, With Safari Technology Preview’" href="https://daringfireball.net/linked/2021/09/25/try-safari-15-tech-preview">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Daring Fireball Weekly Sponsorships for Q4</title>
<link rel="alternate" type="text/html" href="https://daringfireball.net/feeds/sponsors/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tog"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/24/df-sponsorships-q4"/>
<id>tag:daringfireball.net,2021:/linked//6.38464</id>
<published>2021-09-24T23:30:00Z</published>
<updated>2021-09-25T17:00:27Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Sponsorships have been selling briskly this year, but I’ve only just now opened spots for the October-December quarter. <s><em>Plus</em>, a last-minute change has opened up next week’s spot, starting this coming Monday.</s></p> <p>One sponsor per week, with a sponsor-written entry in the RSS feed to start the week, a thank-you post right on the homepage from me at the end, and the one and only graphic ad on every page of the site all week long. No tracking or other privacy-invasive bullshit. Just plain honest ads. That’s not new — that’s the way the ads on DF have <a href="https://daringfireball.net/2004/09/sponsor_this">always been</a>. My best argument that they work: <a href="https://daringfireball.net/feeds/sponsors/archive">the number of repeat companies in the sponsor archive list</a>.</p> <p>So if you’ve got a product or service you’d like to promote to DF’s discerning audience, <a href="mailto:sponsors@daringfireball.net?subject=Feed%20Sponsorship">I’d love to have you as a sponsor</a>. <s>And if you’re ready to grab next week’s opening, let’s go — should be another good week.</s></p> <div> <a title="Permanent link to ‘Daring Fireball Weekly Sponsorships for Q4’" href="https://daringfireball.net/linked/2021/09/24/df-sponsorships-q4">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>‘Float’</title>
<link rel="alternate" type="text/html" href="https://www.youtube.com/watch?v=H8qFTgcRV6w"/>
<link rel="shorturl" type="text/html" href="http://df4.us/toa"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/24/float"/>
<id>tag:daringfireball.net,2021:/linked//6.38458</id>
<published>2021-09-24T23:29:00Z</published>
<updated>2021-09-25T17:14:42Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Aundre Larrow, announcing his directorial debut:</p> <blockquote> <p>Shot on the new iPhone 13 Pro, <em>Float</em> is a short film about the journey that a father and daughter take together.</p> </blockquote> <p>If this doesn’t move you, you’re not hooked up right. Good god, what a powerful, lovely, beautiful short film. Headphones and full screen — this deserves your attention. I <a href="https://daringfireball.net/2021/09/the_iphones_13#cinematic_mode">take it back</a>, Cinematic mode — <a href="https://twitter.com/aundrelarrow/status/1441025854977417224">which Larrow used to shoot this</a> — is no gimmick at all.</p> <p>This is just astonishing. Remember Aundre Larrow’s name.</p> <div> <a title="Permanent link to ‘‘Float’’" href="https://daringfireball.net/linked/2021/09/24/float">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>iPhone Day Is Still a Thing</title>
<link rel="alternate" type="text/html" href="https://vimeo.com/613966202"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tof"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/24/iphone-day"/>
<id>tag:daringfireball.net,2021:/linked//6.38463</id>
<published>2021-09-24T23:06:43Z</published>
<updated>2021-09-27T23:08:50Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>I shot this video while walking past the Philly Apple Store at 2 pm. The line went most of the way down the block. I’ll bet the line was longer than it would have been without COVID restrictions, but still — this is the 15th generation of iPhones and people are <a href="https://daringfireball.net/linked/2017/11/03/iphone-x-campout">still</a> lining up to buy them on the day they’re available. And how many <em>more</em> people had them delivered today, waking up early a week ago to preorder the moment the online store came online? People love the iPhone. If you look at it solely as a technology product you’re missing the biggest part of the iPhone story. iPhone Day is a de facto annual holiday for untold millions of people <a href="https://www.apple.com/newsroom/2021/09/iphone-13-lineup-new-ipad-mini-and-ninth-generation-ipad-arrive-worldwide/">around the world</a>.</p> <p>That’s not true of any other product in the world.</p> <div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/613966202?h=444a7a0f19&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="iPhone Day 2021, Philadelphia"></iframe></div> <script src="https://player.vimeo.com/api/player.js"></script> <div> <a title="Permanent link to ‘iPhone Day Is Still a Thing’" href="https://daringfireball.net/linked/2021/09/24/iphone-day">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Apple’s iOS Changes Are Hurting Facebook’s Ad Business</title>
<link rel="alternate" type="text/html" href="https://www.cnbc.com/2021/09/24/apples-ios-changes-hurt-facebooks-ad-business.html"/>
<link rel="shorturl" type="text/html" href="http://df4.us/toe"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/24/apple-facebook-kantrowitz"/>
<id>tag:daringfireball.net,2021:/linked//6.38462</id>
<published>2021-09-24T22:01:34Z</published>
<updated>2021-09-24T22:01:34Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Alex Kantrowitz, writing for CNBC:</p> <blockquote> <p>“Just completely running blind” is how Aaron Paul, a performance Facebook marketer, described it. Paul said his company, Carousel, moved from spending millions of dollars each day on Facebook to a few hundred thousand dollars. Before the iOS changes, Facebook generated 80% of the traffic Carousel sent to its product pages. Now it accounts for 20%.</p> <p>Apple’s iOS changes may lead to irreparable harm to Facebook’s ad business. This moment has demonstrated to Paul and his fellow performance buyers that relying on one channel (albeit a very effective one) is risky. So they’re looking to diversify their ad spend. Paul said he’s moved his ad budget elsewhere, including “<a href="https://www.cnbc.com/quotes/SNAP">Snapchat</a> and TikTok, but also silent killers like email.” On <a href="https://www.cnbc.com/quotes/TWTR">Twitter</a>, Facebook marketers discussing Apple’s changes <a href="https://twitter.com/search?q=https%3A%2F%2Ftwitter.com%2Fsoundslikecanoe%2Fstatus%2F1440117176132935683&amp;src=typed_query">almost unanimously agreed</a> they needed to follow suit.</p> </blockquote> <p>🎻.</p> <div> <a title="Permanent link to ‘Apple’s iOS Changes Are Hurting Facebook’s Ad Business’" href="https://daringfireball.net/linked/2021/09/24/apple-facebook-kantrowitz">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Another Sign of Microsoft Establishing ‘Surface’ as a Standalone Brand</title>
<link rel="alternate" type="text/html" href="https://surface.com/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/toh"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/24/surface-brand"/>
<id>tag:daringfireball.net,2021:/linked//6.38465</id>
<published>2021-09-24T22:00:00Z</published>
<updated>2021-09-25T20:10:42Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>To <a href="https://daringfireball.net/linked/2021/09/23/surface-event-highlights">my point yesterday</a> about Microsoft establishing “Surface” as a brandname, sans “Microsoft” as a prefix — the headline on the Surface homepage (which redirects from surface.com): “New laptops from Surface, now with Windows 11”.</p> <div> <a title="Permanent link to ‘Another Sign of Microsoft Establishing ‘Surface’ as a Standalone Brand’" href="https://daringfireball.net/linked/2021/09/24/surface-brand">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>App Store Release Notes of the Week: Poolsuite FM</title>
<link rel="alternate" type="text/html" href="https://twitter.com/gruber/status/1441423424337764362"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tod"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/24/poolsuite-fm-release-notes"/>
<id>tag:daringfireball.net,2021:/linked//6.38461</id>
<published>2021-09-24T17:49:43Z</published>
<updated>2021-09-24T17:49:44Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>This is the most joyful way of saying “We’re sorry our iOS 15 compatibility update was a few days late” I can imagine. What a fun app.</p> <div> <a title="Permanent link to ‘App Store Release Notes of the Week: Poolsuite FM’" href="https://daringfireball.net/linked/2021/09/24/poolsuite-fm-release-notes">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Monotype Acquires Hoefler&Co.</title>
<link rel="alternate" type="text/html" href="https://www.typography.com/blog/monotype-acquires-hoeflerco"/>
<link rel="shorturl" type="text/html" href="http://df4.us/toc"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/24/monotype-hoefler"/>
<id>tag:daringfireball.net,2021:/linked//6.38460</id>
<published>2021-09-24T15:51:05Z</published>
<updated>2021-09-26T19:13:56Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Jonathan Hoefler:</p> <blockquote> <p>Nothing’s changing at typography.com, where you’ll still find all 1,113 fonts in the Hoefler&amp;Co library, as well as the cloud.typography webfont service, and all the other resources we’ve created for designers and brands. The H&amp;Co team is staying in place, too, and there are yet more typefaces from us that you can look forward to seeing soon. […]</p> <p>In the meantime, I’ll be stepping down from my role in the company, to finally make the time to recharge, reflect, and explore some new ideas. In these past few years, <a href="https://www.typography.com/blog/abstract-typography-episode">participating in a documentary</a> and using typography to help <a href="https://www.typography.com/blog/biden-fonts">elect a president</a> have been potent reminders of just how many ways there are for type to make a difference, and just how many people are moved by the splendor of typography.</p> </blockquote> <p>I’d need 144-point type to express my surprise at this announcement.</p> <div> <a title="Permanent link to ‘Monotype Acquires Hoefler&amp;Co.’" href="https://daringfireball.net/linked/2021/09/24/monotype-hoefler">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>iPhone 13 Pro Works, But Fits Poorly With MagSafe Duo Charger</title>
<link rel="alternate" type="text/html" href="https://twitter.com/MKBHD/status/1441086122839339015"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tob"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/24/iphone-13-pro-magsafe-duo"/>
<id>tag:daringfireball.net,2021:/linked//6.38459</id>
<published>2021-09-24T15:05:08Z</published>
<updated>2021-09-24T15:05:08Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Awkward.</p> <p><em>(Remembers that the MagSafe Duo Charger costs $130.)</em></p> <p><em>Really</em> awkward.</p> <div> <a title="Permanent link to ‘iPhone 13 Pro Works, But Fits Poorly With MagSafe Duo Charger’" href="https://daringfireball.net/linked/2021/09/24/iphone-13-pro-magsafe-duo">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>My Advice on How to Set Up a New iPhone or iPad: Quick Start Device-to-Device Transfer</title>
<link rel="alternate" type="text/html" href="https://support.apple.com/en-us/HT210216"/>
<link rel="shorturl" type="text/html" href="http://df4.us/to9"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/24/how-to-set-up-a-new-iphone-or-ipad"/>
<id>tag:daringfireball.net,2021:/linked//6.38457</id>
<published>2021-09-24T05:14:54Z</published>
<updated>2021-09-25T15:11:57Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>A bunch of you are probably getting new iPhones (and iPads) today. As someone who’s set up 5 new devices in the last week, my advice is to restore a new iPhone with the Quick Start device-to-device transfer, not iCloud backup. Don’t worry if it says it might take a little longer this way, it’s worth it. Get a cup of coffee or a bite to eat. A watched pot never boils; a watched transfer never finishes.</p> <p>Device-to-device is better because it moves over <em>all</em> your login credentials. When you restore from an iCloud backup, you wind up logged out of a <em>lot</em> of apps on the new device. When you restore device-to-device, almost everything moves over. I know there are <a href="https://twitter.com/renefouquet/status/1441259286177325063">exceptions</a>, but I don’t think I bounced into a single app that didn’t keep me fully logged in this week. If you tried device-to-device a few years ago and found it lacking, try it again now — Apple has improved this process every year since it debuted. Worst case scenario, you can always start over and use iCloud backup.</p> <p>Also, you do not need to unpair your Apple Watch from your old iPhone using this method. You can just wear your watch the whole time. When the transfer is complete, the new iPhone will prompt you, asking if you want to move your watch to the new iPhone. Your mileage may vary but it just worked for me.</p> <p><a href="https://twitter.com/gruber/status/1441255208558997506">I posted this on Twitter tonight</a>, and realized I should post about this here too. The Twitter thread has a bunch of Q&amp;A’s about specific apps, like authentication tokens in Authy (they transfer fine).</p> <p><strong>Update, 25 September 2021:</strong> Lots of positive feedback from readers who took my advice. Perfect? No. But I’m more convinced than ever that device-to-device transfer is the way to go. Apple has done a lot of work, year after year, to keep making this migration experience better, faster, simpler, more complete, and more reliable. I see it firsthand, setting up multiple new iOS devices a year. The team behind this doesn’t get enough thanks, so let me say it: thank you.</p> <div> <a title="Permanent link to ‘My Advice on How to Set Up a New iPhone or iPad: Quick Start Device-to-Device Transfer’" href="https://daringfireball.net/linked/2021/09/24/how-to-set-up-a-new-iphone-or-ipad">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Om Malik on the New iPad Mini</title>
<link rel="alternate" type="text/html" href="https://om.co/2021/09/22/the-ipad-mini-2021-review/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/to8"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/23/om-malik-ipad-mini"/>
<id>tag:daringfireball.net,2021:/linked//6.38456</id>
<published>2021-09-23T23:49:28Z</published>
<updated>2021-09-24T14:31:46Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Om Malik:</p> <blockquote> <p>The best way to extract the most out of the smallest iPad is to think of it as a device enhanced by non-keyboard input methods — Scribble with Pencil, snapping photos with the cameras, or using Siri/voice input. The improved “Scribble” allows you to make notes, do quick searches, and even find directions. It is a very addictive way to use the iPad, especially in the smaller size. […]</p> <p>The more I use the device, the more I realize that most computing has been defined by a singular idea of work and productivity. Mobile devices have and will continue to redefine our work. In the past, most of the computing involved being in the office. Now, non-office tasks have access to computing resources and thus offer an opportunity to make them more productive. Devices like the iPad are about making non-office work a bit more productive. Whether it is doctors, field engineers, or delivery drivers, devices such as the iPad in general and iPad Mini, in particular, could help change the very notion of productivity.</p> </blockquote> <p>What makes Om’s perspective interesting to me is that he switched to an iPad Pro as his main computer a few years back, and loves it. The iPad Mini isn’t an alternative to those sort of use cases — but as he points out, there are so many things people do with “computers” today that just weren’t imagined even a decade ago.</p> <p>I’m sort of the anti-Om in this regard. I have a 2018 iPad Pro that I generally keep in my kitchen, connected to a Magic Keyboard. <a href="https://daringfireball.net/2020/04/the_ipad_magic_keyboard">Ever since the Magic Keyboard came out</a> (with trackpad support and good keyboard shortcut support in iPadOS), I’ve found the iPad Pro <em>much</em> more useful for my work. But nowhere near as useful as a Mac. I’m not arguing that a MacBook is better than an iPad for work. I’m just saying MacOS works better for me. Not even close. Getting in the flow on my Mac, I feel 10 times more productive than I ever do on my iPad Pro. But the iPad Pro with Magic Keyboard is good enough that I now suspect it leads me to punt around in the kitchen drinking coffee <em>much</em> longer than I should at the start of my workdays. I like an iPad for reading the news at the start of the day, but I might be better served with a more limited iPad Mini than a significantly more useful iPad Pro with Magic Keyboard, just because it’d push me to get to my office and sit my ass in front of my real work machine.</p> <div> <a title="Permanent link to ‘Om Malik on the New iPad Mini’" href="https://daringfireball.net/linked/2021/09/23/om-malik-ipad-mini">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>The Microsoft Event Had In-Person Hands-On Time With Products</title>
<link rel="alternate" type="text/html" href="https://twitter.com/caro_milanesi/status/1440709608608202756"/>
<link rel="shorturl" type="text/html" href="http://df4.us/to7"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/23/microsoft-event-was-in-person"/>
<id>tag:daringfireball.net,2021:/linked//6.38455</id>
<published>2021-09-23T23:41:48Z</published>
<updated>2021-09-24T05:29:48Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Carolina Milanesi, on Twitter:</p> <blockquote> <p>I had the opportunity to see the new @surface devices live … and I am so glad I did.</p> <p>Holding #SurfaceDuo in my hand, seeing the clever case that secures the #SurfacePen that looks like a finish rather than a case not adding any thickness, the fluidity of the screen and the clever gaming controls…. Very much looking forward to giving it a spin!</p> </blockquote> <p>Amen to this enthusiasm for seeing the product introduction live. I get it why Apple did not hold an in-person press event last week — iPhone events are <em>huge</em>, and while I think small events can safely be held in person now, there’s no practical way to shrink the iPhone event.</p> <p>I miss having hands-on time with new devices as soon as keynotes end. You pick up on things immediately: that something is heavier or lighter than you expected. That certain colors or finishes look different. Remember the Jet Black iPhone 7? You <em>had</em> to see it in person to understand how it looked. And I miss in-person briefings, both official ones and unofficial. In-person communication simply cannot be beaten for conveying subtlety.</p> <p>Product reviews are hampered too. With in-person Apple events, most reviewers get kit in the hours after the keynote ends. With virtual Apple events, the kit ships for delivery the next day. An extra day makes a big difference when the review embargo drops just one week after the event.</p> <div> <a title="Permanent link to ‘The Microsoft Event Had In-Person Hands-On Time With Products’" href="https://daringfireball.net/linked/2021/09/23/microsoft-event-was-in-person">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Highlights From Microsoft’s Fall Surface Event</title>
<link rel="alternate" type="text/html" href="https://www.theverge.com/2021/9/22/22684950/microsoft-surface-event-biggest-announcements-pro-8-duo-studio-laptop"/>
<link rel="shorturl" type="text/html" href="http://df4.us/to6"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/23/surface-event-highlights"/>
<id>tag:daringfireball.net,2021:/linked//6.38454</id>
<published>2021-09-23T23:26:05Z</published>
<updated>2021-09-24T06:17:35Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Nice supercut video from The Verge squeezing Microsoft’s Surface event yesterday into eight minutes. A few thoughts:</p> <p>It seems like Microsoft is letting the Surface division stand on its own, brand-wise. They’re not distancing themselves from Microsoft in any way, but branding-wise they’re just letting the products be the “Surface Whatever”, not the “Microsoft Surface Whatever”. There’s even a moment in the event, regarding the folding Duo 2 phone, when a guy says it has “the most precise and reliable hinge mechanism ever engineered at Surface”. I.e. that it was “Surface” who engineered that hinge, not “Microsoft”. I think Surface works as a Microsoft sub-brand like that.</p> <p>Speaking of the Surface Duo 2 — their folding phone with two screens — they’re now just calling it what they should have called it all along: a phone. It’s a very interesting and unique form factor, but it’s a big folding phone, not a small folding tablet. It supposedly has real cameras this time, too. Starting price: $1,500.</p> <p>The new Surface Laptop Studio looks really dumb to me. I don’t understand why one would ever want to use it in either of the new folding positions. I guess maybe if you really want to draw on it, you might want to fold it flat, but if you really want to draw that much, why not buy the Surface Pro 8 that detaches from the keyboard? This design <a href="https://www.theverge.com/2021/9/23/22688432/microsoft-surface-laptop-studio-book-3-specs-step-backwards">just seems dumb</a>.</p> <p>The Surface Slim Pen 2 introduces haptic feedback, to simulate the feel of a pen on paper. I love stuff like that.</p> <div> <a title="Permanent link to ‘Highlights From Microsoft’s Fall Surface Event’" href="https://daringfireball.net/linked/2021/09/23/surface-event-highlights">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Apple Watch Series 7 Supports 60.5GHz Wireless Data Transfer, Perhaps Only for Apple’s Internal Use</title>
<link rel="alternate" type="text/html" href="https://www.macrumors.com/2021/09/23/apple-watch-60-5-ghz-wireless-data-transfer/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/to5"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/23/series-7-wireless-data-transfer"/>
<id>tag:daringfireball.net,2021:/linked//6.38453</id>
<published>2021-09-23T22:13:08Z</published>
<updated>2021-09-24T05:04:52Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Joe Rossignol, reporting for MacRumors:</p> <blockquote> <p>Apple Watch Series 7 models are equipped with a new module that enables 60.5GHz wireless data transfer, according to <a href="https://www.scribd.com/document/527108597/Apple-Watch-Series-7-FCC-Filing">FCC filings</a> viewed by MacRumors, but this functionality may be reserved for Apple’s internal use only for now.</p> <p>The filings indicate that the 60.5GHz module is only activated when the Apple Watch is placed on a proprietary magnetic dock with a corresponding 60.5GHz module, but this dock will likely be reserved for use by Apple employees. For example, it’s possible that Apple Stores might use the dock to wirelessly restore an Apple Watch, and if so, it will be interesting to see if Series 7 models still have a hidden diagnostic port for wired connectivity.</p> </blockquote> <p>This is a little interesting in and of itself. But if you look at the long-term trend, it’s a sign that Apple — along with the rest of the industry — is moving toward wireless technology for both charging <em>and</em> data transfer. Apple Watch exemplifies that — it’s <em>never</em> had a port, either for charging or data. There’s a diagnostic port hidden inside the bottom channel for the watch strap, but those <em>diagnostics</em> are neither charging nor data.</p> <p>It’s long been my guess that iPhone is never going to support USB-C. I think it’s Apple’s intention to go straight from Lightning to wireless/inductive, with no “port”. Portless is the future for all devices. Yet the product design geniuses at the European Commission want to mandate all devices have one specific port in 2024 and indefinitely thereafter — a port that by that time <a href="https://en.wikipedia.org/wiki/USB-C">will already be 10 years old</a>.</p> <div> <a title="Permanent link to ‘Apple Watch Series 7 Supports 60.5GHz Wireless Data Transfer, Perhaps Only for Apple’s Internal Use’" href="https://daringfireball.net/linked/2021/09/23/series-7-wireless-data-transfer">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>European Commission Unveils Long-Awaited Stupid Proposal to Mandate USB-C on All Cell Phones and Devices</title>
<link rel="alternate" type="text/html" href="https://www.nytimes.com/2021/09/23/business/european-union-apple-charging-port.html"/>
<link rel="shorturl" type="text/html" href="http://df4.us/to4"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/23/eu-usbc-mandate"/>
<id>tag:daringfireball.net,2021:/linked//6.38452</id>
<published>2021-09-23T21:41:34Z</published>
<updated>2021-09-24T01:09:01Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Elian Peltier, reporting for The New York Times:</p> <blockquote> <p>The European Union unveiled plans on Thursday to make USB-C connectors the standard charging port for all smartphones, tablets and other electronic devices sold across the bloc, an initiative that it says will reduce environmental waste but that is likely to hit Apple the hardest.</p> <p>The move would represent a long-awaited yet aggressive step into product-making decisions by the European Commission, the bloc’s executive arm. Apple, whose iPhones are equipped with a different port, has long opposed the plan, arguing that it would stifle innovation and lead to more electronic waste as all current chargers that are not USB-C would become obsolete. […]</p> <p>The <a href="https://ec.europa.eu/commission/presscorner/detail/en/ip_21_4613">new legislation</a> is likely to come into effect in 2024 because it first needs to be approved by the European Parliament and then adopted by manufacturers. Besides phones, it would apply to cameras, headphones, portable speakers and video game consoles.</p> </blockquote> <p><a href="https://twitter.com/benedictevans/status/1441009296540676096">Benedict Evans</a>:</p> <blockquote> <p>This is a profoundly stupid way to approach product design and standardisation. What happens in 5 years when someone wants to use a better connector? What if they’d picked USB 3 five years ago?</p> </blockquote> <p>How stupid? This stupid:</p> <blockquote> <p>But Apple has also argued that if the European Union had imposed a common charger in 2009, it would have restricted innovation that led to USB-C and Lightning connectors. In a statement, Apple said that although it welcomed the European Commission’s commitment to protecting the environment, it favored a solution that left the device side of the charging interface open for innovation.</p> <p>Mr. Breton said on Thursday that he was familiar with Apple’s concerns. “Every time we try to put a proposal, such companies start to say, ‘It will be against innovation,’” he said.</p> <p>“It’s not at all against innovation. It’s not against anyone,” he added. “It’s for European consumers.”</p> <p>Mr. Breton said manufacturers, including Apple, could choose to offer two charging ports on their devices if they wanted to keep a non-USB-C connector.</p> </blockquote> <p>Two charging ports on the same phone, what an elegant idea. This is like a parody of overzealous regulation of something that is not in need of any regulation at all. Why not mandate that all phones, tablets, and cameras have to run the same operating system, too? Oh, you say, it’s only about reducing waste? Why not mandate that all phones must be the same size and shape, so that they’re all compatible with the exact same cases? Great idea.</p> <p>These E.U. meddlers have indeed been clamoring for this legislation since 2009 — Apple didn’t pick that date out of the air. At the time, iPhones used 30-pin iPod USB 1 adapters and most other phones used adapters like Micro-USB and (gag) Mini-USB. You don’t have to be a computer engineer to look back at your lifetime and realize that computer plugs and adapters keep getting smaller and better. Do they really think no one is going to come up with an adapter better than USB-C? Ever?</p> <p>And don’t even start with any sort of argument that legislation like this won’t impede progress, but will instead force the industry to work together via committee to agree upon new better standards in a prompt fashion. Almost everything that goes through such committees takes <em>years</em> longer than one company can do on its own, and comes out worse — often far worse. <a href="https://en.wikipedia.org/wiki/USB#Receptacle_(socket)_identification">Look at all the horrendously shitty USB plugs</a> the USB consortium has come up with over the years.</p> <p>And people in the E.U. wonder why England wanted out, and why nearly all the major tech companies are from the U.S. and Asia.</p> <div> <a title="Permanent link to ‘European Commission Unveils Long-Awaited Stupid Proposal to Mandate USB-C on All Cell Phones and Devices’" href="https://daringfireball.net/linked/2021/09/23/eu-usbc-mandate">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Austin Mann’s iPhone 13 Pro Camera Review: Tanzania</title>
<link rel="alternate" type="text/html" href="https://austinmann.com/trek/iphone-13-pro-camera-review-tanzania"/>
<link rel="shorturl" type="text/html" href="http://df4.us/to3"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/23/mann-mckay-iphone-13-tanzania"/>
<id>tag:daringfireball.net,2021:/linked//6.38451</id>
<published>2021-09-23T21:10:47Z</published>
<updated>2021-09-23T21:12:10Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>No big deal — just a safari expedition to Tanzania. Lions, leopards, giraffes. Ultra wide angle 4K 60 video shot from an iPhone 13 Pro mounted to a helicopter. Your typical iPhone camera review.</p> <p>The review starts with a terrific movie — including some truly pro-looking Cinematic mode shots — by <a href="https://mckayfilms.com">Taylor McKay</a>.</p> <p>I thought this was a pretty interesting observation from Mann:</p> <blockquote> <p>Although the iPhone 13 Pro still only has three lenses, the addition of macro capability is like adding a new lens altogether, and for the serious photographer I think it’s perhaps the strongest advancement in this year’s camera system. […]</p> <p>Photographer or not, you’ve seen the big and heavy backpacks photographers carry with them on every shoot. Whether it’s local or international, we lug these bags full of lenses around because each one offers a new perspective on whatever story it is that we’re telling.</p> <p>As a photographer passionate about the natural world, I carry a macro lens with me no matter what project I’m working on, just because I never know what tiny detail of interest might present itself. Now with the macro capability of the iPhone 13 Pro, I feel like I have my “in-a-pinch” macro shots covered and I can leave the rarely-used macro lens at home.</p> </blockquote> <p>Everything you see in this video was shot with a $1,000 device meant to fit in your pocket.</p> <p>Some great iOS 15 tips from Mann, too, including using the new Focus feature to create a custom “Shoot Mode” with no notifications whenever he’s using the Camera app or Halide. Also, Mann’s custom Photographic Style settings.</p> <div> <a title="Permanent link to ‘Austin Mann’s iPhone 13 Pro Camera Review: Tanzania’" href="https://daringfireball.net/linked/2021/09/23/mann-mckay-iphone-13-tanzania">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Software Update Adds Bluetooth Audio Support to the Nintendo Switch, Four Years After It Debuted</title>
<link rel="alternate" type="text/html" href="https://twitter.com/NintendoAmerica/status/1437930124490457088"/>
<link rel="shorturl" type="text/html" href="http://df4.us/to2"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/23/nintendo-switch-bluetooth-audio-finally"/>
<id>tag:daringfireball.net,2021:/linked//6.38450</id>
<published>2021-09-23T20:34:19Z</published>
<updated>2021-09-23T20:37:45Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>A story like this is why you shouldn’t misuse <em>finally</em> in headlines. Four years!</p> <div> <a title="Permanent link to ‘Software Update Adds Bluetooth Audio Support to the Nintendo Switch, Four Years After It Debuted’" href="https://daringfireball.net/linked/2021/09/23/nintendo-switch-bluetooth-audio-finally">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>How Apple Built the iPhone 13’s Cinematic Mode</title>
<link rel="alternate" type="text/html" href="https://techcrunch.com/2021/09/23/how-apple-built-the-iphone-13-pros-cinematic-mode/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/to1"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/23/panzarino-cinematic-mode"/>
<id>tag:daringfireball.net,2021:/linked//6.38449</id>
<published>2021-09-23T20:18:32Z</published>
<updated>2021-09-23T20:28:03Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Great interview by Matthew Panzarino with Apple vice president Kaiann Drance and human interface designer Johnnie Manzari from Apple’s Camera team:</p> <blockquote> <p>That’s not even counting tracking shots, where a focus puller is continually adjusting focus as the camera moves and even the subject moves in relation to the camera. It’s a highly skilled operation. To pull off a tracking shot, a focus puller must practice and train extensively for years. This, Manzari says, is where Apple sees an opportunity.</p> <p>“We feel like this is the kind of thing that Apple tackles the best. To take something difficult and conventionally hard to learn, and then turn it into something automatic and simple.”</p> <p>So the team started working through the technical problems in finding focus, locking focus and racking focus. And these explorations led them to gaze.</p> <p>“In cinema, the role of gaze and body movement to direct that story is so fundamental. And as humans we naturally do this, if you look at something, I look at it too.”</p> <p>So they knew they would need to build in gaze detection to help lead their focusing target around the frame, which in turn leads the viewer through the story. Being on set, Manzari says, allowed Apple to observe these highly skilled technicians and then build in that feel.</p> </blockquote> <p>Panzarino includes <a href="https://www.youtube.com/watch?v=3JcEG5Vjt-w">this three-minute video consisting of nothing but Cinematic mode clips</a> from the trip to Disneyland he took with his family to test the new iPhones. There are some really neat shots in the video — I particularly like the one around the 1m:32s mark with his kids on the carousel. That change in focus is exactly what Cinematic mode was meant for.</p> <p>But the other thing that Panzarino’s video exemplifies is that you don’t have to <em>work</em> to use Cinematic mode. No help from someone else (let alone a crew), no extra lighting, no more difficult than just shooting a regular video mode clip. Something anyone could do — and might want to do — on a hectic day at a fun theme park. If you screw up the focus while shooting you can <em>easily</em> fix it — or just improve it — later. </p> <div> <a title="Permanent link to ‘How Apple Built the iPhone 13’s Cinematic Mode’" href="https://daringfireball.net/linked/2021/09/23/panzarino-cinematic-mode">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Apple’s Texas-Sized Problem</title>
<link rel="alternate" type="text/html" href="https://popular.info/p/apples-texas-problem"/>
<link rel="shorturl" type="text/html" href="http://df4.us/to0"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/23/apple-texas-sized-problem"/>
<id>tag:daringfireball.net,2021:/linked//6.38448</id>
<published>2021-09-23T18:58:55Z</published>
<updated>2021-09-23T21:19:25Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Judd Legum, writing at Popular Information:</p> <blockquote> <p>On Friday, CEO Tim Cook answered a question about Apple’s stance on the Texas ban at an <a href="https://www.nytimes.com/2021/09/17/technology/apple-employee-unrest.html">all-staff meeting</a>. Cook said that “the company was looking into whether it could aid the legal fight against the new law.”</p> <p>Apple has considerable leverage over the abortion debate in Texas and across the country — but it is not related to its ability to pay for lawyers. Apple’s leverage rests in its status as a major employer and driver of economic growth.</p> <p>If Apple believes that its employees should be able to “make their own decisions regarding their reproductive health,” it could publicly state that it will not expand its workforce in states that limit abortion rights. That would have a major influence not only in Texas but in <a href="https://popular.info/p/in-key-states-corporate-donations">numerous states considering following Texas’ lead</a>.</p> </blockquote> <p>Last week, <a href="https://techcrunch.com/2021/09/16/in-internal-memo-apple-says-it-is-monitoring-legal-challenges-to-texas-abortion-law/">TechCrunch published the text of a company-wide memo</a> posted to an internal Apple message board regarding Texas’s near-outlawing of abortion. It began:</p> <blockquote> <p>A message about women’s reproductive health care</p> <p>At Apple, we support our employees’ rights to make their own decisions regarding their reproductive health.</p> </blockquote> <p>Legum is right — it’s untenable for Apple, or any other company, to “support our employees’ rights to make their own decisions regarding their reproductive health” <em>and</em> ask any woman to work for the company in a state with a law like Texas’s. An immediate hiring and construction freeze in Texas — explicitly tied to this outrageous law (which makes no exceptions for rape or incest) — is the only tenable action compatible with Apple’s stated values.</p> <p><a href="https://twitter.com/AoDespair/status/1439957619901411329">David Simon, linking to Legum’s post</a>:</p> <blockquote> <p>If an employer, this is beyond politics. I’m turning in scripts next month on an HBO non-fiction miniseries based on events in Texas, but I can’t and won’t ask female cast/crew to forgo civil liberties to film there. What else looks like Dallas/Ft. Worth?</p> </blockquote> <p>That’s the answer. You move your business out of Texas. Any company that expands or initiates new operations in Texas implicitly supports Texas’s abortion ban.</p> <div> <a title="Permanent link to ‘Apple’s Texas-Sized Problem’" href="https://daringfireball.net/linked/2021/09/23/apple-texas-sized-problem">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<link rel="alternate" type="text/html" href="https://daringfireball.net/2021/09/epic_apple_developer_accounts"/>
<link rel="shorturl" href="http://df4.us/tnz"/>
<id>tag:daringfireball.net,2021://1.38447</id>
<published>2021-09-23T01:29:18Z</published>
<updated>2021-09-23T03:50:58Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<summary type="text">Accounts that have never been disabled include the accounts for Rocket League (a game whose Mac support [Epic discontinued in January 2020][rl]), and separately, Unreal Engine. My understanding is that none of those accounts are affected by Apple’s decision not to reinstate the Fortnite developer account.</summary>
<content type="html" xml:base="https://daringfireball.net/" xml:lang="en">
<![CDATA[ <p><a href="https://twitter.com/timsweeneyepic/status/1440711772483186690">Tim Sweeney, today on Twitter</a>:</p> <blockquote> <p>Late last night, Apple informed Epic that Fortnite will be blacklisted from the Apple ecosystem until the exhaustion of all court appeals, which could be as long as a ]]>
<![CDATA[ 5-year process.</p> </blockquote> <p>Sweeney posted a letter from Apple’s attorneys to Epic’s. It reads:</p> <blockquote> <p>September 21, 2021</p> <p>VIA ELECTRONIC MAIL</p> <p>Gary Bornstein <br /> Cravath, Swaine &amp; Moore LLP <br /> Worldwide Plaza <br /> 825 Eighth Avenue <br /> New York, NY 10019-7475</p> <p>Re: Developer Program Account No. 8XJ6WJ8Z84</p> <p>Dear Gary,</p> <p>I am responding to your recent request that Apple reinstate Epic’s developer program account, which was terminated for cause last year. Epic committed an intentional breach of contract, and breach of trust, by concealing code from Apple and making related misrepresentations and omissions. In its decision, the court recognized that “Apple had contractual rights to act as It did. It merely enforced those rights as [Epic’s] own internal documents show Epic Games expected.” ECF No. 812 at 178-79. The court further found that “Apple’s termination of the [Developer Program License Agreement] and the related agreements between Epic Games and Apple was valid, lawful, and enforceable.” <em>Id.</em> at 179. Following that decision, Mr. Sweeney has publicly said that Epic “[w]ouldn’t trade [an alternative payment system] away to get Fortnite back on iOS.” In light of this and other statements since the court’s decision, coupled with Epic’s duplicitous conduct in the past, Apple has exercised its discretion not to reinstate Epic’s developer program account at this time. Furthermore, Apple will not consider any further requests for reinstatement until the district court’s judgment becomes final and nonappealable.</p> <p>Sincerely,</p> <p>/s/ Mark A. Perry <br /> Mark A. Perry</p> </blockquote> <p>That’s lawyer-speak, I believe, for “go fuck yourselves”.<sup id="fnr1-2021-09-22-B"><a href="#fn1-2021-09-22-B">1</a></sup></p> <p><a href="https://twitter.com/TimSweeneyEpic/status/1440711467888615431">Sweeney is crying foul</a>, arguing that this contradicts Apple’s repeated public statements that Fortnite would be welcomed back to the App Store <em>if they came into full compliance with App Store rules</em>. Here’s a version of Apple’s statement from two weeks ago, <a href="https://www.protocol.com/apple-blocks-epic-from-bringing-fortnite-back-to-the-app-store">via Protocol</a>:</p> <blockquote> <p>“As we’ve said all along, we would welcome Epic’s return to the App Store if they agree to play by the same rules as everyone else. Epic has admitted to breach of contract and as of now, there’s no legitimate basis for the reinstatement of their developer account.”</p> </blockquote> <p>Apple’s lawyers’ characterization of Sweeney’s statement about being unwilling to trade something away “to get Fortnite back on iOS” does seem like a bit of a hatchet-job, quote-editing-wise. <a href="https://twitter.com/TimSweeneyEpic/status/1440712310339694592">Sweeney tweeted the following on September 11</a>, one day after the Epic-v.-Apple decision was delivered:</p> <blockquote> <p>Thinking much more about whether we’re going to live in a world where two platform megacorps dictate software and world commerce to everyone or whether the digital world and the future metaverse will be a free world. Wouldn’t trade that away to get Fortnite back on iOS.</p> </blockquote> <p>That doesn’t sound like the words of a man poised to comply with the App Store rules around in-app purchases. But, it doesn’t mean Epic <em>wasn’t</em> going to submit a Fortnite build that fully complies with the rules, either. Really does seem like Sweeney just thinking out loud in a tweet.</p> <p>Sweeney <em>also</em> <a href="https://twitter.com/TimSweeneyEpic/status/1440711578819567622">tweeted an email</a> he sent to Phil Schiller on September 16. It reads:</p> <blockquote> <p>From: Tim Sweeney <br /> Date: Thu, Sep 16, 2021 at 5:01 PM <br /> Subject: Fortnite and the App Store <br /> To: Phil Schiller </p> <p>Hi Phil,</p> <p>I’m writing to provide clarity on where we stand.</p> <p>Epic has appealed the court’s decision in our suit over Apple’s policies on In-App Purchase and competing stores. Though we can’t update the Fortnite version that users still have on their iOS devices, we’ve disabled Epic payments server-side, and have paid Apple $6,000,000 as ordered by the court.</p> <p>Epic has asked Apple to reactivate our Fortnite development account. Epic promises that it will adhere to Apple’s guidelines whenever and wherever we release products on Apple platforms. If we get the account back, we’ll bring Fortnite back to Mac as soon as possible, and we’ll reincorporate Fortnite for iOS in our Unreal Engine development and testing process, which will benefit all of our mutual developers.</p> <p>Whether Epic chooses to bring Fortnite back to iOS consumers depends on whether and where Apple updates its guidelines to provide for a level playing field between Apple In-App Purchase and other methods of payment.</p> <p>Epic will resubmit Fortnite to the App Store if you adhere to the plain language of the court order and allow apps to include buttons and external links that direct customers to other purchasing mechanisms without onerous terms or impediments to a good user experience. In that case, our remaining dispute will be about competing stores, and I genuinely believe we could find common ground on the topic if Apple’s position were based solely on user security and privacy rather than commercial interests.</p> <p>As a provider of developer tools, Epic continues to support Apple platforms and our mutual developers wholeheartedly.</p> <p>If you have any questions or thoughts, I’m happy to talk.</p> <p>Tim Sweeney <br /> Epic Games</p> </blockquote> <p>A few comments:</p> <blockquote> <p>Epic promises that it will adhere to Apple’s guidelines whenever and wherever we release products on Apple platforms.</p> </blockquote> <p>Epic, of course, had previously promised the same thing, in a legally binding fashion, when they agreed to Apple’s developer account terms and conditions. But agreeing not to break Apple’s guidelines again seems in the spirit of what Apple had been asking for, regarding reinstating Fortnite.</p> <blockquote> <p>Epic will resubmit Fortnite to the App Store if you adhere to the plain language of the court order and allow apps to include buttons and external links that direct customers to other purchasing mechanisms without onerous terms or impediments to a good user experience.</p> </blockquote> <p>Here’s where I think Sweeney garnered the legal “go fuck yourself”. Sweeney is arguing that Apple, which won the lawsuit, should interpret <a href="https://stratechery.com/2021/the-apple-v-epic-decision/">the court’s anti-steering injunction</a> in a way that pleases Epic, which lost the lawsuit. That’s not how things work.</p> <blockquote> <p>In that case, our remaining dispute will be about competing stores, and I genuinely believe we could find common ground on the topic if Apple’s position were based solely on user security and privacy rather than commercial interests.</p> </blockquote> <p>Tim Sweeney is high as a kite.</p> <hr /> <p>So here’s the thing to keep in mind, and that I think Sweeney purposefully muddled in the way he announced this news: Epic is a conglomerate with multiple subsidiaries, and those subsidiaries have their own Apple Developer Program accounts. The only developer account Apple ever disabled in this dispute was the one held by Epic Games, Inc. — the Fortnite account. It was disabled on 28 August, 2020 and has been disabled ever since.</p> <p>Accounts that have never been disabled include the accounts for Rocket League (a game whose Mac support <a href="https://www.rocketleague.com/news/ending-support-for-mac-and-linux/">Epic discontinued in January 2020</a>, exemplifying Epic’s “wholehearted” support for “Apple platforms”), and separately and importantly, Unreal Engine. It <em>is</em> true that Apple moved to block the Unreal Engine account back in August 2020, <a href="https://techcrunch.com/2020/08/24/apple-ordered-to-not-block-epic-games-unreal-engine-but-fortnite-to-stay-off-app-store/">but Judge Yvonne Gonzalez Rogers ordered Apple not to pending a decision in the case</a>, while allowing the Fortnite account to be blocked. In her ruling this month, however, Gonzalez Rogers stated that Apple would now be within its rights to disable any and all of Epic’s Apple developer accounts for breaching the license agreement. (See p. 179 of <a href="https://daringfireball.net/linked/2021/09/10/judgment-in-epic-v-apple">the ruling</a>.)</p> <p>My understanding is that none of those accounts are affected by Apple’s decision not to reinstate the Fortnite developer account. Those accounts have been operational throughout this legal dispute, and I believe will continue to be — by Apple’s choice.</p> <div class="footnotes"> <hr /> <ol> <li id="fn1-2021-09-22-B"> <p>Thank goodness lawyers seemingly always let you know in ALL CAPS when they send a letter via email, that they in fact SENT IT VIA ELECTRONIC MAIL.&nbsp;<a href="#fnr1-2021-09-22-B" class="footnoteBackLink" title="Jump back to footnote 1 in the text.">&#x21A9;&#xFE0E;</a></p> </li> </ol> </div> ]]>
</content>
<title>★ Apple Will Not Reinstate Epic’s Fortnite Developer Account, but Epic’s Other Developer Accounts Remain Active</title>
</entry>
<entry>
<title>iPhone 13 and Apple Silicon</title>
<link rel="alternate" type="text/html" href="https://creativestrategies.com/iphone-13-and-apple-silicon/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tny"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/22/bajarin-iphone-13-apple-silicon"/>
<id>tag:daringfireball.net,2021:/linked//6.38446</id>
<published>2021-09-22T23:59:05Z</published>
<updated>2021-09-23T00:16:10Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Ben Bajarin, writing at Creative Strategies:</p> <blockquote> <p>While I will admit there is a small percentage of Apple customers who upgrade every year and a percentage more who upgrade every two years because they are on upgrade plans, the vast majority of consumers upgrade every 3-4 years. I thought it would be interesting to look at some basic iPhone benchmarks through the years and look at how much performance improvement happens every four years.</p> </blockquote> <p>Incremental improvements every year turn into profound improvements over 3–4 years. It’s like the technology version of compound interest. It adds up.</p> <blockquote> <p>As I benchmarked the A15 Bionic in different ways and pondered how Apple spends its transistor budget with each A-series chip cycle, an interesting shift emerged for iPhone 13. Going back to how Apple spends their transistor budget on features, not necessarily performance, for the A15, Apple looks to have had the most GPU gains YoY since the A9. For the past five years, Apple has had an average of 19% GPU gains YoY but for the A15 Bionic, <em>Apple has increased GPU performance by 52%</em>.</p> <p>This intentional increase in GPU performance over CPU performance speaks to the more graphically intense features Apple had in mind for iPhone 13 that is demonstrated in things like macro photography, macro video, and Cinematic Mode. Developers also now have a dramatically increased GPU at their disposal to create new app experiences around and can leverage new augmented reality techniques, visual computing and AI, and more.</p> </blockquote> <p>It’s almost enough to make one think that Apple is ready to release high-end professional Macs built around Apple GPUs.</p> <div> <a title="Permanent link to ‘iPhone 13 and Apple Silicon’" href="https://daringfireball.net/linked/2021/09/22/bajarin-iphone-13-apple-silicon">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Music Video Shot With iPhone 13 Pro Cinematic Mode: Julia Wolf — ‘Falling in Love’</title>
<link rel="alternate" type="text/html" href="https://www.youtube.com/watch?v=Ae19-qqIMbQ"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnx"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/22/cinematic-mode-morrison-video"/>
<id>tag:daringfireball.net,2021:/linked//6.38445</id>
<published>2021-09-22T22:58:40Z</published>
<updated>2021-09-22T22:58:40Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Jonathan Morrison:</p> <blockquote> <p>Went hands on with the iPhone 13 Pro and immediately wanted to test out the camera and cinematic mode. It’s limited to 1080p 30fps but I was surprised to see how sharp it was AND that it retained Dolby Vision.</p> </blockquote> <p>Interesting to see Cinematic mode in the hands of a talented videographer. Easily the best “in the wild” Cinematic mode video I’ve seen. (Explicit lyrics in the song.)</p> <div> <a title="Permanent link to ‘Music Video Shot With iPhone 13 Pro Cinematic Mode: Julia Wolf — ‘Falling in Love’’" href="https://daringfireball.net/linked/2021/09/22/cinematic-mode-morrison-video">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Wired’s 2011 Review of the iPhone 4S</title>
<link rel="alternate" type="text/html" href="https://www.wired.com/2011/10/iphone4s/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnw"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/22/wired-2011-iphone-4s-review"/>
<id>tag:daringfireball.net,2021:/linked//6.38444</id>
<published>2021-09-22T22:07:39Z</published>
<updated>2021-09-22T22:08:14Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>From Wired’s review of the iPhone 4S:</p> <blockquote> <p>Apple never specified what the “S” stands for in iPhone 4S, and it may as well stand for Siri. Sure, the fifth-generation iPhone’s superb camera and speedy dual-core processor are classy additions. But Siri is the reason people should buy this phone. […]</p> <p>The iPhone 4S looks exactly the same as its predecessor — but who cares? If it was shaped even slightly differently or came in a new color, people would still go nuts over the stuff that’s more important anyway: the insides. And both inside and out, this is a magnificent smartphone.</p> <p>The late Steve Jobs once called the computer the equivalent of a bicycle for our minds. I think of the smartphone as the rocket ship for our minds. With increasingly powerful sensors and technologies, and access to hundreds of thousands of apps enabling us to do just about anything, the iPhone keeps soaring to incredible heights and taking us to places with limitless potential. I guess that’s what you have to do to create a ding in the universe.</p> </blockquote> <p>I don’t know what happened to the fellow who wrote this review 10 years ago, but The New York Times <a href="https://daringfireball.net/linked/2021/09/22/review-from-another-planet">could sure use</a> a personal tech critic with this sort of enthusiasm and insight into the way that incremental improvements aggregate in just a few years in profound ways.</p> <div> <a title="Permanent link to ‘Wired’s 2011 Review of the iPhone 4S’" href="https://daringfireball.net/linked/2021/09/22/wired-2011-iphone-4s-review">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>‘The Most Important iPhone Ever’</title>
<link rel="alternate" type="text/html" href="http://www.asymco.com/2021/09/21/the-most-important-iphone-ever/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnv"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/22/dediu-most-important-iphone-ever"/>
<id>tag:daringfireball.net,2021:/linked//6.38443</id>
<published>2021-09-22T21:35:10Z</published>
<updated>2021-09-23T00:07:29Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Horace Dediu, writing at Asymco:</p> <blockquote> <p>There are more than 1 billion iPhone users. The total number of users has been rising steadily. iPhone users make up about 26% of all smartphone users (3.8 billion is the current estimate). The share of users in the US is about 60% (or soon will be.) The share in UK is close to 50%. All these share numbers are higher than ever. Over 14% of US and 10% of UK survey respondents have switched to an iPhone in the past two years.</p> </blockquote> <p>I was not aware that churn was so strongly in the favor of iPhone over the last two years. Pretty good for a phone that <a href="https://daringfireball.net/linked/2012/01/24/blodget">Henry Blodget declared “dead in the water”</a> in 2012. The downside to this trend, if it continues, is Apple might start running into being deemed an actual monopolist — by which I mean holding a monopoly share of <em>phones</em> period, not just a monopoly on iPhones. And with its sole OS competitor <a href="https://daringfireball.net/linked/2020/06/25/wong-ios-14-android">increasingly showing signs</a> of <a href="https://daringfireball.net/linked/2020/07/20/state-of-google-pixel">losing institutional interest</a> in Android, that trend might continue.</p> <p>Dediu on the iPhone 13 and Apple’s camera improvements over the last few years in general:</p> <blockquote> <p>We did not ask for rack focus, post-production focus (!), night mode, macro photography and portrait bokeh. But once we have these features we begin, ever so slowly, to use them and then we start demanding them. Conversely it seems that what people mostly ask for — that is what the critics ask for — are extrapolations of existing features. The “faster horse” dilemma.</p> </blockquote> <p>On the surface, the physics of photography are stacked against Apple. Apple’s “cameras” are pancake-thin phones that people rightfully expect to comfortably carry in a jeans pocket. The technically-best photos and videos you can create today are shot using very large, very heavy cameras. But in a very meaningful way, this severe disadvantage works in Apple’s favor. It’s good to be the underdog. It keeps you hungry. And in photography, Apple is very much the underdog — not to any competing company but to the laws of physics. They’ve been making better smartphones than their competition since the day the first iPhone went on sale. That can make a company lazy, and lose focus. The worst thing that ever happened to the Mac was Microsoft Windows going to shit after Windows XP. </p> <p>But Apple will be chasing “real” cameras in image quality for at least another decade, maybe forever. Settling for nothing less than making the best cameras, period, despite the severe form factor constraints of a “phone”, is the sort of north star that keeps a company focused.</p> <div> <a title="Permanent link to ‘‘The Most Important iPhone Ever’’" href="https://daringfireball.net/linked/2021/09/22/dediu-most-important-iphone-ever">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<link rel="alternate" type="text/html" href="https://daringfireball.net/2021/09/the_2021_ipad_mini"/>
<link rel="shorturl" href="http://df4.us/tnu"/>
<id>tag:daringfireball.net,2021://1.38442</id>
<published>2021-09-22T18:58:16Z</published>
<updated>2021-09-23T00:04:47Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<summary type="text">I think most iPad Mini fans would have been delighted if the new model were specced *exactly* like the current iPad Air, at these same prices. That the iPad Mini offers several technical advantages over last year’s iPad Air is pure gravy.</summary>
<content type="html" xml:base="https://daringfireball.net/" xml:lang="en">
<![CDATA[ <p>I don’t generally lead with benchmarks or pricing, but here’s a thought about the new iPad Mini, which comes equipped with a version of the same A15 chip as the new iPhone 13 and 13 Pro models: For $500, you can buy an iPad that’s more or less as fast, if not faster, at single-threaded CPU performance as an M1 Mac.</p> <p>That’s a tremendous value. The iPad Mini even has an A15 with an extra (fifth) GPU core, like the iPhone 13 Pro.</p> <p>Upgrading from 64 to 256 GB of storage costs $150; upgrading to add cellular support costs $150. So a maxed out iPad Mini — 256 GB of storage plus cellular support — costs $800. (There are only two storage options, 64 and 256 GB.) It’d be nice if — like all the new iPhone 13 models — the base storage were 128 GB instead of 64. But, still, the new iPad Mini is a terrific little tablet, and has performance that should keep it very useful for many years to come.</p> <p>It is, effectively, an iPad <em>Air</em> Mini. <a href="https://www.apple.com/ipad/compare/?modelList=ipad-air-4th-gen,ipad-mini-6th-gen,ipad-9th-gen">Just like the iPad Air</a>, the new Mini sports a round-cornered display, no home button, and Touch ID on the power button. The new no-adjective entry-level iPad still has a square-cornered display, and Touch ID on a traditional home button on the front face. Also like the current iPad Air, the new iPad Mini uses a USB-C port instead of Lightning, and thus uses the superior magnetic second-generation Apple Pencil.</p> <p>Because the Mini is brand new and the current Air came out last October, the Mini was able to pull ahead in certain respects: A15 instead of A14, 5G support on cellular models, and a better front-facing camera (12 MP vs. 7 MP) — including support for <a href="https://support.apple.com/en-us/HT212315">Center Stage</a>, Apple’s recent feature that dynamically adjusts the front-facing camera’s field of view depending on how many people are in the frame and where they are. The rear cameras of the Air and Mini are similarly specced, and to my eyes shoot equivalent quality photos and video, but the new iPad Mini includes True Tone LED flash. The big win to me is the upgraded front-facing camera with Center Stage support. I’m not sure if you’ve heard, but video calls have become a big deal over the last two years.</p> <p>I think most iPad Mini fans would have been delighted if the new model were specced <em>exactly</em> like the current iPad Air, at these same prices. (The iPad Air costs $100 more than the equivalent Mini for the same amount of storage — $600 for 64 GB, $750 for 256 GB — but it only costs $130 to add cellular support to the Air. I suspect the difference in cellular model pricing is a 5G thing.) That the iPad Mini offers several technical advantages over last year’s iPad Air is pure gravy.</p> <p>I’ve been using the new iPad Mini for a week. As is my tradition for reviews of and first looks at new iPad models, I’m <a href="/misc/2021/09/ipad-mini-k2-keyboard-magic-trackpad.jpeg">writing this piece on the iPad Mini itself</a>, using <a href="https://www.keychron.com/products/keychron-k2-wireless-mechanical-keyboard">a bluetooth keyboard</a> and Magic Trackpad. It’s a nice small-footprint setup. The smaller text on the Mini’s smaller display is a little hard on my aging and somewhat problematic eyes while sitting at hardware keyboard distance, but my biggest annoyance is the lack of Face ID. I’m spoiled by my 2018 iPad Pro — while using a keyboard with an iPad, I expect to both wake it up <em>and</em> unlock it by just pressing the space bar or any other key. Having to reach over and touch the Touch ID button on the iPad is, simply, an inferior experience compared to Face ID. And it’s especially hard for me, right now, after a few years of expecting Face ID to just work with an iPad connected to a keyboard. I felt the same way writing <a href="https://daringfireball.net/2020/10/the_2020_ipad_air">last year’s piece on the iPad Air</a>.</p> <p>If you don’t already have a Face ID habit using your iPad, however, this should be no big deal at all. Perhaps it’s even unfair for me to complain about, given that I do the vast majority of my writing on an M1 MacBook Pro — which also uses Touch ID, not Face ID. But maybe it <em>is</em> fair to complain about, because on a MacBook the Touch ID button is right on the keyboard — much more convenient to reach — and Macs support unlocking via the proximity of your Apple Watch. I think it’d be very cool if iPadOS supported unlocking via Apple Watch, much like MacOS does.</p> <p>All that said, if you’re the sort of person who’d like to do a lot of writing on an iPad Mini, you’ll be fine.</p> <p>One interesting change is that the hardware volume buttons have moved to the same side of the device as the power/Touch ID button. That means the volume buttons are on top when the iPad is in vertical orientation, and on the left side of the device when horizontal. The reason for this is obvious when you think about it, and consider the size of an Apple Pencil. Speaking in vertical (a.k.a. portrait) orientation terms, the Pencil, when attached, doesn’t leave any room for volume buttons on the right side of the device. But the volume buttons can’t go on the left side, because they’d get covered up when you connect a cover (like Apple’s own Smart Folio, which is very nice — the English lavender Smart Folio that Apple provided me with pairs nicely with the purple iPad Mini.) So, the volume buttons moved.</p> <p>One quibble: there are a few aspects of iPadOS that to me feel optimized only for larger iPads. The home screen Dock, for example, accepts up to 16 apps and folders. In vertical orientation, those icons are <em>really</em> tiny. Almost comically so. Yet in the same orientation, iPadOS will only display 5 apps in the Command-Tab switcher when you have a keyboard connected. I’m more annoyed by having just 5 apps in the Command-Tab switcher than by having super-small icons in my Dock, because I can adjust the number of apps in my Dock (by dragging a few lesser-used ones out) but I can’t adjust the maximum number of apps in the Command-Tab switcher. <a href="/misc/2021/09/ipad-mini-dock-versus-switcher.jpeg">Here’s a screenshot</a>, but viewing it on another device won’t do justice to the feeling of just how small those Dock icons are, and just how comfortably a few more apps could fit in the switcher. It’s hard to put a finger on it,<sup id="fnr1-2021-09-22"><a href="#fn1-2021-09-22">1</a></sup> but there are just certain visual elements in iPadOS that feel inconsiderately shrunken on the iPad Mini, in a way that is <em>not</em> true for iOS on an iPhone Mini.</p> <p>A corresponding anti-quibble: After a fairly long stretch of not using an iPad Mini, I’m reminded how much nicer I find this size for typing with the on-screen keyboard compared to my 11-inch iPad Pro, because I can type with my thumbs, iPhone-style. I have never taken to typing on-screen on an iPad with my fingers, touch-typing-style, and at this point — over a decade into the iPad era — I doubt I ever will. As with the iPhone, I wouldn’t want to write anything long-form using just my thumbs on the on-screen keyboard, but it’s fine for dashing off text messages, tweets, and short emails. And, even better: <a href="https://twitter.com/gruber/status/1440816307381817346">the iPad Mini still supports splitting the keyboard in two</a>, to make thumb-typing even easier. (It continues to baffle me that the iPad Pros do not support split keyboard mode.) If you like the idea of using an iPad as a sort of big-ass iPhone, the iPad Mini is obviously the iPad for you.</p> <div class="footnotes"> <hr /> <ol> <li id="fn1-2021-09-22"> <p>No pun intended, I swear, vis-à-vis my complaint about tiny icons in the Dock.&nbsp;<a href="#fnr1-2021-09-22" class="footnoteBackLink" title="Jump back to footnote 1 in the text.">&#x21A9;&#xFE0E;</a></p> </li> </ol> </div> ]]>
</content>
<title>★ The 2021 iPad Mini</title>
</entry>
<entry>
<title>Who Needs to Shoot Photos in Low Light Anyway?</title>
<link rel="alternate" type="text/html" href="https://twitter.com/reckless/status/1440309785295933447"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnt"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/22/review-from-another-planet"/>
<id>tag:daringfireball.net,2021:/linked//6.38441</id>
<published>2021-09-22T14:48:29Z</published>
<updated>2021-09-22T22:18:29Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Nilay Patel, on Brian X. Chen’s iPhone 13 review for <s>Pravda</s> The New York Times:</p> <blockquote> <p>The NYT does not believe regular people stand to benefit from better iPhone photos in the dark. I live for this review from another planet every year.</p> </blockquote> <p>I thought this was a really strange passage too. Quoting from <a href="https://www.nytimes.com/2021/09/21/technology/personaltech/apple-iphone13-review.html">Chen’s review</a>:</p> <blockquote> <p>So in summary, the iPhone 13 cameras are slightly better than those of last year’s iPhones. Even compared with iPhones from three years ago, the cameras are much better only if you care about taking nice photos in the dark.</p> <p>Just how important is night photography? I posed the question to Jim Wilson, a longtime staff photographer for The New York Times, as he was taking pictures of the new iPhones for this review. He said it would be a crucial feature for people like him, but not as important for casual shooters.</p> </blockquote> <p>I enjoy how Chen’s review opens with an egalitarian slam that Apple and Samsung’s annual phone updates are “a mirage of tech innovation” and instead are “a celebration of capitalism”, but when it comes to explaining why typical users shouldn’t care about low-light photography, he basically says “<em>because a professional staff photographer at The New York Times says they shouldn’t care</em>”.</p> <p><a href="https://twitter.com/benthompson/status/1440601049245491200">Ben Thompson recalled</a> (as <a href="https://daringfireball.net/2019/09/you_could_always_just_use_flash">I should have</a>, but did not) that this is something of a recurring theme. From <a href="https://www.nytimes.com/2019/09/17/technology/personaltech/iphone-11-review.html">Chen’s review of the iPhones 11 and 11 Pro two years ago</a>:</p> <blockquote> <p>Photos taken with the iPhone 11 and 11 Pro looked crisp and clear, and their colors were accurate. But after I finished these tests, I looked back at my archived photos taken with an iPhone X.</p> <p>Those pictures, especially the ones shot with portrait mode, still looked impressive. Some of the low-light ones looked crummy in comparison with the ones taken by the iPhone 11s, but I wouldn’t recommend that you buy a new phone just to get better night photos. You could always just use flash.</p> </blockquote> <p>“<em>You shouldn’t feel the need to buy a new iPhone every year</em>” is a fine sentiment, one that many, if not most, reviewers make each year. Arguing, repeatedly, that your readers should not be concerned at all about taking better photos in low light is bizarre. The single biggest change in consumer photography over the last 3–4 years is the exponential improvement in low light and night mode photography on new mobile phones.</p> <p>And again, <a href="https://daringfireball.net/linked/2021/09/21/chen-iphones-13">as I mentioned yesterday</a>, Chen’s iPhone 13 review doesn’t even mention battery life, even though almost every other reviewer noted significant improvements across the lineup.</p> <div> <a title="Permanent link to ‘Who Needs to Shoot Photos in Low Light Anyway?’" href="https://daringfireball.net/linked/2021/09/22/review-from-another-planet">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Brian X. Chen on the iPhones 13: ‘The Most Incremental Upgrade Ever’</title>
<link rel="alternate" type="text/html" href="https://www.nytimes.com/2021/09/21/technology/personaltech/apple-iphone13-review.html"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tns"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/21/chen-iphones-13"/>
<id>tag:daringfireball.net,2021:/linked//6.38440</id>
<published>2021-09-21T22:44:36Z</published>
<updated>2021-09-21T22:44:36Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Brian X. Chen’s review of the new iPhones for The New York Times is the least enthusiastic I’ve seen:</p> <blockquote> <p>This is all to say the annual phone upgrade, which companies like Apple and Samsung tout with enormous marketing events and ad campaigns to gin up sales for the holiday shopping season, has become a mirage of tech innovation. In reality, the upgrades are now a <a href="https://www.nytimes.com/2021/08/12/technology/new-smartphone-models.html">celebration of capitalism</a> in the form of ruthless incrementalism.</p> </blockquote> <p>Fair enough, but I found it curious that Chen’s review didn’t contain the word “battery”. The <a href="https://www.techmeme.com/210921/p18#a210921p18">consensus is pretty strong</a> that the two standout features are better cameras and improved battery life.</p> <div> <a title="Permanent link to ‘Brian X. Chen on the iPhones 13: ‘The Most Incremental Upgrade Ever’’" href="https://daringfireball.net/linked/2021/09/21/chen-iphones-13">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Joanna Stern: ‘From Mini to Pro Max, It’s All About the Battery and Cameras’</title>
<link rel="alternate" type="text/html" href="https://www.wsj.com/articles/iphone-13-pro-max-mini-review-11632223198"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnr"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/21/stern-iphone-13-cinematic-mode"/>
<id>tag:daringfireball.net,2021:/linked//6.38439</id>
<published>2021-09-21T21:32:16Z</published>
<updated>2021-09-21T21:32:16Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Joanna Stern, reviewing the iPhone 13 lineup for the WSJ:</p> <blockquote> <p>With videos, gosh, I was really excited about the new Cinematic mode. Aaaand gosh, was it a let down. The feature — which you could call “Portrait mode for video” — adds artistic blur around the object in focus. The coolest thing is that you can tap to refocus while you shoot (and even do it afterward in the Photos app).</p> <p>Except, as you can see in my video, the software struggles to know where objects begin and end. It’s a lot like the early days of Portrait Mode, but it’s worse because now the blur moves and warps. I shot footage where the software lost parts of noses and fingers, and struggled with items such as a phone or camera. The Apple spokeswoman said Cinematic mode is a “breakthrough innovation that will keep getting better over time.”</p> </blockquote> <p>Stern went all-in on Cinematic mode for the video accompanying her review.</p> <div> <a title="Permanent link to ‘Joanna Stern: ‘From Mini to Pro Max, It’s All About the Battery and Cameras’’" href="https://daringfireball.net/linked/2021/09/21/stern-iphone-13-cinematic-mode">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Raymond Wong’s iPhone 13 Pro Review for Input</title>
<link rel="alternate" type="text/html" href="https://www.inputmag.com/reviews/iphone-13-pro-max-review-a-mighty-upgrade-thats-just-shy-of-perfect"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnq"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/21/wong-iphone-13-pro"/>
<id>tag:daringfireball.net,2021:/linked//6.38438</id>
<published>2021-09-21T21:04:19Z</published>
<updated>2021-09-22T14:17:43Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Raymond Wong shot a bunch of great camera comparisons for his Input review. He was annoyed by the same jarring automatic switch between the 1× to 0.5× lens when entering or leaving macro mode that I mentioned <a href="https://daringfireball.net/2021/09/the_iphones_13">in my review</a>:</p> <blockquote> <p>I welcome greater detail for close-ups and it’s clever that Apple is using the ultra-wide to augment the 1× wide and 3× telephoto at short distances, but the transitioning of cameras is disorienting. Apple makes no mention of this camera switching/augmenting on its iPhone 13 Pro website. I get that it’s supposed to be one of those “it just works” features. At least that was Apple’s intention I’m told, but it just doesn’t.</p> <p>Here’s a screen recording of the automatic camera switching in action. In this shot, I was trying to frame these delicious soup dumplings using the grid. Holding the iPhone 13 Pro still, you can see the 1× wide switching to another slightly different FOV that’s using the ultra-wide autofocusing. The viewfinder keeps jittering as it tries to choose between a regular wide or wide-macro shot. A regular person wouldn’t look at this and think to themselves, this is <em>normal</em>. They’d look at the jittering and think something is broken with their iPhone camera. The framing should <em>never</em> change from what you compose and never automatically.</p> </blockquote> <p>Wong’s screen recording illustrates the issue perfectly.</p> <blockquote> <p>When I first pressed Apple and made them aware of the jarring camera switching, I was told it’s how the camera system works. On the eve of this review, Apple changed course and said it’s going to release a software update to let users disable the camera switching. According to Apple:</p> <blockquote> <p>A new setting will be added in a software update this fall to turn off automatic camera switching when shooting at close distances for macro photography and video.</p> </blockquote> </blockquote> <div> <a title="Permanent link to ‘Raymond Wong’s iPhone 13 Pro Review for Input’" href="https://daringfireball.net/linked/2021/09/21/wong-iphone-13-pro">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Panzarino Takes the iPhone 13 Pro to Disneyland</title>
<link rel="alternate" type="text/html" href="https://techcrunch.com/2021/09/21/the-iphone-13-pro-goes-to-disneyland/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnp"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/21/panzarino-iphone-13-disneyland"/>
<id>tag:daringfireball.net,2021:/linked//6.38437</id>
<published>2021-09-21T20:54:31Z</published>
<updated>2021-09-21T20:54:32Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Matthew Panzarino, writing for TechCrunch, regarding Cinematic video mode:</p> <blockquote> <p>I did some test shooting with my kids walking through crowds and riding on carousels that was genuinely, shockingly good. It really does provide a filmic, dreamy quality to the video that I was previously only able to get with quick and continuous focus adjustments on an SLR shooting video with a manually focused lens.</p> <p>That, I think, is the major key to understanding Cinematic Mode. Despite the marketing, this mode is intended to unlock new creative possibilities for the vast majority of iPhone users who have no idea how to set focal distances, bend their knees to stabilize and crouch-walk-rack-focus their way to these kinds of tracking shots. It really does open up a big bucket that was just inaccessible before. And in many cases I think that those willing to experiment and deal with its near-term foibles will be rewarded with some great looking shots to add to their iPhone memories widget.</p> </blockquote> <p>That sounds right to me.</p> <div> <a title="Permanent link to ‘Panzarino Takes the iPhone 13 Pro to Disneyland’" href="https://daringfireball.net/linked/2021/09/21/panzarino-iphone-13-disneyland">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>Dieter Bohn on the iPhone 13 Pro</title>
<link rel="alternate" type="text/html" href="https://www.theverge.com/22684033/apple-iphone-13-pro-max-review"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tno"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/21/bohn-iphone-13-pro"/>
<id>tag:daringfireball.net,2021:/linked//6.38436</id>
<published>2021-09-21T20:28:32Z</published>
<updated>2021-09-21T20:28:49Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Dieter Bohn, writing for The Verge:</p> <blockquote> <p>Apple’s marketing for the camera system on the 13 Pro is that it’s the “biggest advancement ever.” I don’t know that I would go that far, but I also can’t remember the last time I’ve said “whoa, look at this photo” as many times as I have during this review. […]</p> <p>Where the Pro 13 camera system shines is in low light. The main wide-angle sensor has seen a massive upgrade this year. Unlike Android phones that are chasing big megapixel counts and then “pixel binning” to achieve low light performance, Apple is sticking with 12 megapixels, the same resolution it’s used since 2015’s iPhone 6S. The sensor itself is much bigger now and features 1.9 µm pixels, which are about as big as anything we’ve seen on a smartphone. And on top of all that, the lens now has an ƒ/1.5 aperture.</p> <p>All of that adds up to a camera that can very quickly take in a massive amount of light relative to other phones. Combined with some tuning and improvements to Apple’s computational photography, the low light performance on the 13 Pro is simply second to none.</p> </blockquote> <p>I came away super impressed with the low light performance of the 13 Pro, too.</p> <p>Bohn makes an important point in <a href="https://www.theverge.com/22684421/apple-iphone-13-mini-review">his corresponding review of the 13 and 13 Mini</a> too: because the camera bumps are all new sizes, cases for the iPhone 13 won’t fit the 13 Pro, nor vice-versa.</p> <div> <a title="Permanent link to ‘Dieter Bohn on the iPhone 13 Pro’" href="https://daringfireball.net/linked/2021/09/21/bohn-iphone-13-pro">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>More, Smaller Apps</title>
<link rel="alternate" type="text/html" href="https://www.apple.com/newsroom/2021/08/apple-acquires-classical-music-streaming-service-primephonic/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnn"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/21/more-smaller-apps"/>
<id>tag:daringfireball.net,2021:/linked//6.38435</id>
<published>2021-09-21T19:06:46Z</published>
<updated>2021-09-21T19:06:47Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Apple Newsroom, back on August 30:</p> <blockquote> <p>Primephonic is no longer available for new subscribers and will be taken offline beginning September 7. Apple Music plans to launch a dedicated classical music app next year combining Primephonic’s classical user interface that fans have grown to love with more added features. In the meantime, current Primephonic subscribers will receive six months of Apple Music for free, providing access to hundreds of thousands of classical albums, all in Lossless and high-resolution audio, as well as hundreds of classical albums in Apple Music’s Spatial Audio, with new albums added regularly.</p> </blockquote> <p>I’ve had this flagged for a few weeks. What I find interesting is Apple is going to use this acquisition to launch a dedicated classical music app, not to expand the Music app. iTunes, infamously, expanded greatly over the years, and everyone seems to agree that the user experience suffered for it. I wonder if that’s in the back of Apple’s mind here.</p> <div> <a title="Permanent link to ‘More, Smaller Apps’" href="https://daringfireball.net/linked/2021/09/21/more-smaller-apps">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<link rel="alternate" type="text/html" href="https://daringfireball.net/2021/09/the_iphones_13"/>
<link rel="shorturl" href="http://df4.us/tnm"/>
<id>tag:daringfireball.net,2021://1.38434</id>
<published>2021-09-21T17:13:47Z</published>
<updated>2021-09-24T14:16:45Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<summary type="text">Computational photography is upending the entire camera world. It’s hard to beat the physics of good glass and large sensors, but math is doing pretty good — and gaining fast.</summary>
<content type="html" xml:base="https://daringfireball.net/" xml:lang="en">
<![CDATA[ <p>I wish I had something more clever to say about the new iPhone 13 lineup. But the practical reality is simple and obvious. The two ways that Apple could best improve the day-to-day utility of using an iPhone are improving the camera system and improving battery life. And those are exactly where Apple focused its attention for this year’s new iPhones.</p> <p>In theory, another practical improvement would be to make phones that are thinner and lighter. But designing phones that are thinner and lighter would be in direct conflict with improving the cameras and battery life. You can’t have your cake and eat it too.</p> <p>All four new iPhones — the 13 Mini, the regular 13, the 13 Pro, and the 13 Pro Max — are the exact same height and width as the corresponding models from last year’s iPhone 12 lineup. But all four of the new iPhones are slightly thicker and heavier. The increase in thickness is very slight — from 7.4 mm to 7.65 mm. The increase in weight varies from around 5 to 7 percent. Not a lot, but you can feel it.</p> <p>The model with the biggest physical change year-over-year is the 6.1-inch 13 Pro. (Apple provided me with all four for testing, but I’ve spent most of my time over the last six days using the 13 Pro.) Last year, <a href="https://daringfireball.net/2020/11/the_iphone_12_mini_and_iphone_12_pro_max">the 12 Pro Max had a much bigger camera module</a> on the back — bigger lenses that protrude more, and a bigger “platform” (“plateau”?) in which the lenses sit. This year, the 13 Pro and 13 Pro Max share the same camera module. You can both see and feel the difference on the 13 Pro compared to last year’s 12 Pro, or to any other previous iPhone in the “regular” size class.</p> <p>It is comical to look back at the minor controversy surrounding the iPhone 6 back in 2014. That was the first year the iPhone camera had a “bump”, which at the time seemed weird and obtrusive, even if the reason for the bump was obvious: improved optics. The controversy was that <a href="https://www.theverge.com/2014/9/16/6209759/apple-has-an-embarassing-bulge">Apple’s promotional photography for the iPhone 6 seemed to go out of its way to hide that camera bump</a> — in a bunch of Apple’s profile shots, the back of the iPhone 6 looked perfectly flat. Apple deliberately chose angles and perspectives that did not show the camera bump, and headlines described the camera — that tiny little iPhone 6 camera — as an “embarrassing bulge”.</p> <p>Fast forward to today, and Apple is using photographs for the iPhone 13 Pro and Pro Max, that, if anything, <em>emphasize</em> the camera system’s size and prominence. Here’s a screenshot from <a href="https://www.apple.com/iphone-13-pro/">Apple’s iPhone 13 Pro product page</a>:</p> <p><a href="/misc/2021/09/iphone-13-pro-camera-bump.jpeg" class="noborder"> <img src = "/misc/2021/09/iphone-13-pro-camera-bump.jpeg" alt = "A promotional photo of a silver iPhone 13 Pro emphasizing the prominence of its camera lenses." width = 450 /></a></p> <p>Nobody can claim Apple is hiding this “bump”. As with the 12 Pro Max last year, the camera systems on the 13 Pro and 13 Pro Max protrude so far that Apple’s cases for the devices have a prominent protective plastic lip around the camera cutout, such that even in a case, the iPhone wobbles when lying on a flat surface. (The cases for the iPhone 13 and 13 Mini have lips around the camera now, too, but they’re much smaller.)</p> <p>I’ve been arguing for years that iPhones are evolving such that they’re better thought of as cameras than “phones”. Now, there’s no need to argue about it. That’s especially true for the Pro models. What’s “pro” about the iPhone 13 Pro and Pro Max? The cameras. The “pro” prefix is right there in the name of camera features exclusive to the Pro devices: <a href="https://support.apple.com/en-us/HT211965">ProRAW</a> and <a href="https://support.apple.com/en-us/HT202410">ProRes</a>. I think it’s fair to say that the iPhone 13 and 13 Mini are phones with very good cameras; the 13 Pro and Pro Max are excellent cameras with phones.</p> <p>Computational photography is upending the entire camera world. It’s hard to beat the physics of good glass and large sensors, but math is doing pretty good — and gaining fast.</p> <h2>Performance, Efficiency, and ProMotion</h2> <p>During Apple’s keynote last week, the company didn’t mention year-over-year performance numbers for the A15 chip. This led to <a href="https://sixcolors.com/link/2021/09/a15-fast-and-slow/">some speculation</a> that maybe the A15 isn’t much faster than the A14. But when benchmarks started leaking last week after phones got into reviewers’ hands, they showed performance improvements roughly in line with the improvements from the last few years: about 10 percent faster in single-threaded benchmarks, and about 20 percent faster in multi-threaded. That jibes with the numbers I saw using <a href="https://www.geekbench.com/">GeekBench 5</a> and the web-based <a href="https://browserbench.org/Speedometer2.0/">Speedometer benchmark</a>.</p> <p>Apple doesn’t like to explain itself, but I think they decided against emphasizing traditional benchmark-type figures (“<em>20 percent faster CPU performance, 40 percent faster machine learning</em>”, etc.) not because the A15 fares poorly in such comparisons, but because numbers like that don’t really tell the story of what the A15 is <em>about</em>. The more impressive year-over-year improvements are in battery life, and I think that’s largely about the efficiency of the A15. It is faster than the A14, by reasonable margins, but what’s more impressive is how much longer battery life is, with only a modest increase in device thickness.</p> <p>On the <a href="https://www.apple.com/iphone/compare/">iPhone model comparison page</a>, Apple cites separate battery figures for “Video playback” and “Video playback (streamed)”. That’s something almost everyone does with their phones — stream video. A practical, real-world measure of battery life. Here are the year-over-year streaming video improvements for each of the four iPhones 12 and 13:</p> <ul> <li>iPhone 13 Mini: 13 hours, up from 10 hours last year on the 12 Mini.</li> <li>iPhone 13: 15 hours, up from 11 hours last year on the regular 12.</li> <li>iPhone 13 Pro: 20 hours, up from 11 hours last year on the 12 Pro.</li> <li>iPhone 13 Pro Max: 25 hours, up from 12 hours last year on the 12 Pro Max.</li> </ul> <p>Those are very big improvements for the non-pro iPhone 13 and 13 Mini. But the numbers for the 13 Pro and Pro Max are bananas. The Pro Max more than doubled its battery life for streaming video playback in a year. (!) All four iPhone 13 models are seeing benefits here from the A15 chip. But the Pro models are benefiting from a surprising direction: ProMotion. That’s Apple’s name for adaptive screen refresh rates. With the iPhone 13 Pro and Pro Max, the screen refresh rate ranges from as low as 10 Hz to as high as 120 Hz, and the system just manages it automatically based on what’s on screen. It’s the high refresh rates that garner attention — it’s a feature that makes scrolling look noticeably smoother. It just looks nicer.<sup id="fnr1-2021-09-21"><a href="#fn1-2021-09-21">1</a></sup> But, of course, updating the display at twice the refresh rate — 120 Hz instead of 60 — obviously consumes more power. </p> <p>This led to some speculation that the iPhone 13 Pro might get <em>worse</em> battery life than the regular iPhone 13, because ProMotion is exclusive to the 13 Pro and Pro Max. That speculation was based on the fact that high-end Android phones with high refresh rates — 90 or 120 Hz — <a href="https://www.anandtech.com/show/15765/120hz-on-the-oneplus-8-pro-qhd-resolution-but-still-power-hungry">take noticeable hits to battery life</a>. What makes ProMotion different is that it’s adaptive. The showy-offy aspect of ProMotion is the high refresh rates, but the undeniable practical benefits are the adaptive <em>lower</em> refresh rates. That’s why the streaming video playback numbers for the 13 Pro and 13 Pro Max effectively doubled year-over-year: stream a video at 30 frames per second, and ProMotion will adapt the display refresh rate to 30 Hz. The adaptive nature of ProMotion means that not only does it not hurt battery life, like the less sophisticated high refresh rate features on Android phones, but it actually helps <em>extend</em> battery life for common tasks like watching video or reading text. Yes, the iPhone is late to the high refresh rate game, but as is often the case with Apple, it was worth waiting for.</p> <h2>Miscellaneous</h2> <ul> <li><p><span id = 'cinematic_mode'>Cinematic video mode</span> is a lot of fun. It’s a gimmick, yes, but I don’t mean that pejoratively. Gimmicks can be fun. Fun is good. I think people are going to use this feature to make videos that really will look more cinematic. It’s also nice that it’s not a feature exclusive to the Pro models. But like Portrait mode for stills, edge detection around subjects’ hair and eyeglasses can be hit or miss in Cinematic mode. Also, I find it a bit curious that Cinematic mode only shoots in one format: 1080p at 30 FPS. The 1080p limitation I understand — the ML-driven automatic subject detection and dynamically-created “bokeh” depth of field effect are clearly computationally expensive. But why not offer 24 FPS too? For reasons that have never been clear to me, Apple’s Camera app has only ever offered 24 FPS at 4K resolution, not at 1080p or 720p. The camera is certainly capable of it — plenty of third-party camera apps let you shoot 24 FPS video at 1080p and 720p, in addition to 4K. But only the system’s Camera app can shoot in Cinematic mode, a mode whose very name suggests “film style”, which is <a href="/misc/2021/09/24fps-film-style.jpeg">exactly the term Apple itself uses in the Settings app to describe 4K 24 FPS</a>.</p></li> <li><p>Macro photography on the iPhone 13 Pro models is also a lot of fun. It’s almost like gaining a super power — the ability to see small objects and details far more clearly than with the naked eye. The way that macro mode kicks in automatically, though, can be a little jarring. How it works is, with a 1× field of view in the regular still photo mode, when you bring the camera very close to a subject or surface, the Camera app switches to the 0.5× ultra wide camera. But it’s not an ultra-wide field of view. You get a roughly 1× field of view but a very close focal distance. The jarring part is when the viewfinder switches between cameras — it’s like a jump cut. It’s understandable, and doesn’t dampen the utility or fun of the feature, but it’s a little weird every time you see it happen. It makes it feel not quite as automatic or modeless as Apple intends it to feel. Also, the built-in Magnifier app (Settings → Accessibility → Accessibility Shortcut) doesn’t seem to use the camera’s macro capability. For reading really tiny text — like, say, some of the <a href="https://www.mentalfloss.com/article/68109/15-microprints-hiding-united-states-currency">hidden fine print on U.S. currency</a> — it’s far easier and more effective to use the Camera app than the Magnifier app.</p></li> <li><p>I bought a regular iPhone 12 last year for my personal use, but I’ve already ordered a 13 Pro this year. (Graphite, of course, because I’m boring that way.) The camera is just too good. Maybe the new 3× telephoto lens just feels like a lot of zoom to me, personally, because I’ve spent the last year mostly using an iPhone 12 that doesn’t have a telephoto lens of any sort, but it really feels like a lot of extra zoom compared even to a 2× iPhone camera from previous years.</p></li> <li><p>Polished stainless steel still feels like an odd material for a phone with flat sides. Somehow, to me, polished steel worked better for the round-sided iPhones (X, XS, 11). With the flat-sided iPhones 12 Pro and now 13 Pro, it’s a fingerprint magnet when used without a case. The aluminum iPhones 13 have better hand-feel to my taste, including the buttons.</p></li> <li><p>Colors: my review units are gold (13 Pro), sierra blue (13 Pro Max), midnight (13 Mini), and blue (regular 13). The gold once again is a very C-3PO gold. Sierra blue is very nice, and quite distinctive from any previous iPhone — I can see why Apple is using it a lot in their advertising. It plays as silver-y at times, but very clearly blue at others. Midnight plays as black or very dark gray, until you put it next to something truly black — it’s then apparent that midnight has a small touch of blue. It makes last year’s black iPhone 12 models look a little drab side-by-side. The non-pro iPhone 13 in just plain blue is nice. It’s a rich, vibrant blue. But <a href="https://daringfireball.net/2020/10/the_iphone_12_and_iphone_12_pro#fn7-2020-10-20">once again</a>, the <a href="/misc/2021/09/no-blue-screws.jpeg">screws on the bottom edge are not color matched</a>. The midnight iPhone 13 Mini has nearly-matching black screws, but the blue iPhone 13 has silver screws. I don’t know why that bugs me.</p></li> <li><p>Battery life was outstanding. As usual, I’ve been using the phone extensively, including power-hungry features like Cinematic mode, and I ended each day with plenty of charge left in the tank.</p></li> </ul> <div class="footnotes"> <hr /> <ol> <li id="fn1-2021-09-21"> <p>It occurred to me while swiping to scroll a long web page as fast as I could that we’re <a href="https://daringfireball.net/2007/06/iphone_first_impressions">a long way removed from the checkerboard placeholder background</a> that Mobile Safari would render while scrolling in iPhone OS version 1.&nbsp;<a href="#fnr1-2021-09-21" class="footnoteBackLink" title="Jump back to footnote 1 in the text.">&#x21A9;&#xFE0E;</a></p> </li> </ol> </div> ]]>
</content>
<title>★ The iPhones 13</title>
</entry>
<entry>
<link rel="alternate" type="text/html" href="https://retool.com/?utm_source=sponsor&utm_medium=newsletter&utm_campaign=daringfireball"/>
<link rel="shorturl" href="http://df4.us/tnl"/>
<link rel="related" type="text/html" href="https://daringfireball.net/feeds/sponsors/2021/09/retool_1"/>
<id>tag:daringfireball.net,2021:/feeds/sponsors//11.38433</id>
<author>
<name>Daring Fireball Department of Commerce</name>
</author>
<published>2021-09-20T19:24:24-05:00</published>
<updated>2021-09-20T19:24:25-05:00</updated>
<content type="html" xml:base="https://daringfireball.net/feeds/sponsors/" xml:lang="en">
<![CDATA[ <p>Programming has gotten surprisingly hard. Building a simple form to POST data back to your API means wrangling with redux and thunks. Oh, and debouncing that submit button. Everything but solving the business problem.</p> <p>Retool is a new approach: we’ve unified the ease of visual programming with the power and flexibility of real code. Drag and drop a form together, and have it POST back to your API in minutes. Deploy instantly with access controls and audit logs.</p> <p>Allbirds uses Retool to measure billboard efficacy. Amazon uses Retool to handle GDPR requests. You, too, can use it to build business-critical applications fast.</p> <p><a href="https://retool.com/?utm_source=sponsor&amp;utm_medium=newsletter&amp;utm_campaign=daringfireball">Start building for free today</a>.</p> <div> <a title="Permanent link to ‘Retool’" href="https://daringfireball.net/feeds/sponsors/2021/09/retool_1">&nbsp;★&nbsp;</a> </div> ]]>
</content>
<title>[Sponsor] Retool</title>
</entry>
<entry>
<title>Listen Notes</title>
<link rel="alternate" type="text/html" href="https://www.listennotes.com/blog/why-podcasts-are-my-new-wikipedia-the-perfect-41/?s=df"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnk"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/18/listen-notes"/>
<id>tag:daringfireball.net,2021:/linked//6.38432</id>
<published>2021-09-18T18:26:43Z</published>
<updated>2021-09-18T18:26:43Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>My thanks to Wenbin Fang for sponsoring this week at DF to promote Listen Notes, a podcast search engine. He sponsored DF to share his story of how listening to podcasts has largely replaced Wikipedia as an informal learning resource for him, personally. </p> <p>Fang has used Listen Notes to help himself listen to about 5,000 podcast episodes in the past 4 years. (!) In his blog post, he explains his own idiosyncratic methods for podcast discovery and consumption.</p> <p>If you want to jumpstart your own podcast project, <a href="https://listennotes.com/api">try the Listen Notes podcast API</a>, or if you want to find all podcast interviews of a person, just search for their name on <a href="https://www.listennotes.com/?s=df">listennotes.com</a>. Just a website, really well done.</p> <div> <a title="Permanent link to ‘Listen Notes’" href="https://daringfireball.net/linked/2021/09/18/listen-notes">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>The Talk Show: ‘It Was More Arial Than Helvetica’</title>
<link rel="alternate" type="text/html" href="https://daringfireball.net/thetalkshow/2021/09/18/ep-322"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnj"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/18/the-talk-show-322"/>
<id>tag:daringfireball.net,2021:/linked//6.38431</id>
<published>2021-09-18T18:17:28Z</published>
<updated>2021-09-18T18:17:29Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Rene Ritchie returns to the show for a recap of this week’s “California Streaming” Apple Event: the iPhones 13, Apple Watch Series 7, and new iPads. Also, last week’s decision in the Apple v. Epic lawsuit.</p> <p>Brought to you by these fine sponsors:</p> <ul> <li><a href="https://squarespace.com/talkshow">Squarespace</a>: Make your next move. Use code <strong>talkshow</strong> for 10% off your first order.</li> <li><a href="https://hellofresh.com/talkshow14">Hello Fresh</a>: America’s #1 meal kit.</li> <li><a href="https://awaytravel.com/talkshow">Away</a>: Designed to last for life.</li> </ul> <div> <a title="Permanent link to ‘The Talk Show: ‘It Was More Arial Than Helvetica’’" href="https://daringfireball.net/linked/2021/09/18/the-talk-show-322">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<link rel="alternate" type="text/html" href="https://daringfireball.net/2021/09/california_streaming_thoughts_and_observations"/>
<link rel="shorturl" href="http://df4.us/tng"/>
<id>tag:daringfireball.net,2021://1.38428</id>
<published>2021-09-15T23:40:00Z</published>
<updated>2021-09-16T09:41:00Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<summary type="text">You’re in luck if you like the color blue.</summary>
<content type="html" xml:base="https://daringfireball.net/" xml:lang="en">
<![CDATA[ <h2>The Event</h2> <p>Staging-wise, I’m not sure I get Apple’s “let’s make this all about California” strategy. The footage from various scenic locations across the state was beautiful, but I don’t get why it mattered for this particular event. Apple’s always been in California, they ]]>
<![CDATA[ ’ve always been proud of being from California. My best guess is that it’s as simple as needing a theme of some sort, and “California scenic beauty” was as good as any, for yet another COVID era event that couldn’t be held inside with an audience. Joz presented outside at Apple Park, and Cook was on stage in the Steve Jobs theater, but I get the feeling they wanted to break away from Apple Park as the set dressing for the whole show, too.</p> <p>To that point, I thought Kaiann Drance’s segment introducing the iPhone 13 and 13 Mini was the most stunning. Standing on stage, alone, at <a href="https://www.sandiegosymphony.org/">the San Diego Symphony’s outdoor theater</a>, in front of <a href="/misc/2021/09/drance-san-diego.jpeg">all those empty seats</a>. It was both beautiful and an instant reminder of what we’re all missing.</p> <h2>The iPhones 13</h2> <p>Last year, the iPhone 12 and 12 Pro — the two “regular” sized new iPhones — shared the exact same protective cases. This year, there are different cases for the iPhone 13 and 13 Pro. I <em>think</em> that’s because the three-lens camera module on the back of the iPhone 13 Pro is bigger than the two-lens module on the iPhone 13. The width, height, and depth of the 13 Pro and regular 13 <a href="https://www.apple.com/iphone/compare/">are identical</a>.</p> <p>Last year, the 12 Pro Max had a better camera system than the 12 Pro. Only the 12 Pro Max had the sensor shift optical image stabilization, and only the 12 Pro Max had a 2.5× (as opposed to 2×) telephoto lens. This year, both Pro models have identical camera systems. (And, like last year, the regular iPhone 13 and 13 Mini share the same camera system as each other.)</p> <p>The iPhone 13 Pro camera modules are entirely different from the non-Pro 13 and 13 Mini, though. Not just the existence of the new 3× telephoto, but the 1× (wide) and 0.5× (ultra wide) cameras are better on the Pro models. The 1× Pro camera has a maximum aperture of ƒ/1.5; the 1× non-Pro camera is ƒ/1.6. (Lower values for aperture let in more light; photographer lingo is that they’re “faster”.) The 0.5× Pro camera has a fast ƒ/1.8 aperture; the 0.5× non-Pro camera is ƒ/2.4.</p> <p>Macro photography is a Pro-only feature, I believe because the 13 Pro 0.5× ultra wide camera has autofocus, and the non-Pro 0.5× camera is fixed-focus.</p> <p>The front-facing camera on all iPhone 13 models appears to be the same, but only the Pro models can shoot in the ProRes format. (Not sure why anyone would want to shoot ProRes with the front-facing camera, though. But I guess why not enable it?)</p> <p>The AI-driven automatic focus changes in Cinematic Mode video seem too good to be true. Very futuristic feature, if it works as promised.</p> <p>I really missed having a hands-on experience with the new devices, if only to consider their colors. “Starlight” appears to be silver with a slight hint of gold. I’m tempted to say champagne, but maybe that implies too much gold. “Midnight” isn’t quite neutral dark gray or near-black — it has a hint of blue or indigo. (Blue is seemingly the color of the year. Anecdotally, it seems like a lot of people I know are planning to get the Pro models in Sierra Blue.)</p> <h2>Apple Watch Series 7</h2> <p>A bigger screen, with a brighter always-on display mode, and faster charging are OK year-over-year improvements. But clearly Series 7 is a minor, not major, refresh. That’s fine, and inevitable for a maturing product. You’re not supposed to buy a new $500 Apple Watch every year, and while I know a lot of people who buy a new iPhone each year (including yours truly), I don’t know anyone, even devout fitness enthusiasts, who buys a new Apple Watch annually. Even every other year feels pretty frequent. A Series 5 or Series 4, purchased new, should still be a really great Apple Watch. [<strong>Update:</strong> I should have known my audience better. A bunch of you buy a new Apple Watch every year. I think we can all admit it’s atypical, though — and that developers who buy a new one every year for testing are an edge case.]</p> <p><a href="https://twitter.com/SnazzyQ/status/1437902520731402242">Quinn “Snazzy Labs” Nelson flagged Apple for an unfair comparison</a>, regarding just how much more text the larger Series 7 displays can show at a time. The font was the same size, but the line spacing was quite a bit tighter in the Series 7 screenshot. I would also argue that Apple chose text that line-wrapped <a href="http://www.eprg.org/G53DOC/pdfs/knuth-plass-breaking.pdf">inefficiently</a> on the Series 6 display, but the difference in line heights is clearly unfair. Apple doesn’t usually play games like that in comparisons. Yellow card issued.</p> <p>The entry model $199 Apple Watch remains the now-kinda-long-in-the-tooth Series 3. I was really hoping for the Series 4 to take that spot in the lineup. I know developers of WatchOS apps were too. The Series 3 has an outdated screen size that developers are going to have to support for years to come.</p> <h2>New iPad Mini and 9th-Generation Just-Plain iPad</h2> <p>The iPad Mini has always been on a unique upgrade cycle. It goes years between refreshes, but when Apple does update it, they tend to bring it up to current specs. The new iPad Mini has the same A15 SoC as the iPhones 13 — in fact, it has the 5-core GPU like the iPhone 13 Pro models, not the 4-core GPU like the iPhone 13 and 13 Mini. The previous iPad Mini had the A12.</p> <p>The iPad Mini is really more like an iPad <em>Air</em> Mini. The new regular “iPad” still has a home button and sharp-cornered display. The Mini has the modern round-cornered display, no home button, and a Touch ID sensor on the power button — just like the current iPad Air. Also like the iPad Air, the new Mini has a USB-C port instead of Lightning. The volume buttons for the Mini are on the top of the device — a first for iPad. I’m guessing that decision was mainly about supporting the magnetic Pencil 2 along the long side of the device where the volume buttons traditionally go for iPads.</p> <h2>TV+ and Fitness+</h2> <p>One thought that occurred to me is that it’s good to see Apple pushing forward on their own original service products. Even putting aside the legal and legislative attention regarding the App Store — big things to put aside, at the moment — I just don’t think it’s healthy for Apple to depend on rent-seeking to grow Services revenue. Getting 30 percent of the revenue from subscriptions to other company’s services is a fine business, financially, but it’s like junk food for any company’s culture. Apple is a great company because they make great original things that people want to pay for. TV+ and Fitness+ are exactly that. Collecting 30 percent of another company’s in-app subscription revenue is not.</p> ]]>
</content>
<title>★ Various Single-Paragraph Thoughts and Observations Regarding Yesterday’s ‘California Streaming’ Apple Event for the iPhones 13, Apple Watch Series 7, and New iPads</title>
</entry>
<entry>
<title>Yours Truly on CNBC This Morning</title>
<link rel="alternate" type="text/html" href="https://www.cnbc.com/video/2021/09/15/john-gruber-apple-embracing-work-from-home-in-latest-product-line.html"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnh"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/15/yours-truly-on-cnbc-this-morning"/>
<id>tag:daringfireball.net,2021:/linked//6.38429</id>
<published>2021-09-15T23:39:31Z</published>
<updated>2021-09-15T23:39:31Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>I enjoy that I’m credited in the headline simply as “expert”. I’ll take that.</p> <div> <a title="Permanent link to ‘Yours Truly on CNBC This Morning’" href="https://daringfireball.net/linked/2021/09/15/yours-truly-on-cnbc-this-morning">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>The Old Last-Minute Hardware Design Switcheroo</title>
<link rel="alternate" type="text/html" href="https://www.cultofmac.com/752777/apple-watch-7-last-minute-substitution/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tnf"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/15/old-last-minute-hardware-switcheroo"/>
<id>tag:daringfireball.net,2021:/linked//6.38427</id>
<published>2021-09-15T16:51:55Z</published>
<updated>2021-09-15T16:51:55Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Killian Bell, writing at Cult of Mac:</p> <blockquote> <p>Apple Watch Series 7 is not the upgrade most of us expected to see from Tuesday’s Apple event. The new model doesn’t sport the big design refresh multiple sources said was coming. It doesn’t even pack a new chip.</p> <p>Is this the upgrade Apple wanted to deliver this year? Or is it a last-minute substitution that Cupertino had to settle on because the refresh it really wanted to deliver just wasn’t ready to roll out?</p> <p>Based on the evidence, we’re going to say it’s the latter.</p> </blockquote> <p>The only way this could be funnier is if Bell included the theory that perhaps Apple changed the hardware at the last minute <em>because</em> the flat-edge designs leaked.</p> <p>This is not how hardware works. These designs are set <em>long</em> in advance. In fact, from what I’ve heard, the flat-edge watch designs might be legitimate leaks, but they’re <em>next</em> year’s designs. That’s how far in advance Apple works on hardware — they were already in the advanced stages of designing the 2022 Apple Watches months ago. (Aesthetically, I am not sold on a flat-edge design for the watch. The round edges are iconic and organic.)</p> <p>You can argue that Series 7 is a marginal upgrade over Series 6, but with an all-new screen (brighter and bigger), all-new crystal (more durable), and 33 percent faster charging, there <em>are</em> upgrades, and none of them could be slapped together.</p> <div> <a title="Permanent link to ‘The Old Last-Minute Hardware Design Switcheroo’" href="https://daringfireball.net/linked/2021/09/15/old-last-minute-hardware-switcheroo">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<title>NSO Group iMessage Zero-Click Exploit Captured in the Wild, Patched by Apple</title>
<link rel="alternate" type="text/html" href="https://citizenlab.ca/2021/09/forcedentry-nso-group-imessage-zero-click-exploit-captured-in-the-wild/"/>
<link rel="shorturl" type="text/html" href="http://df4.us/tne"/>
<link rel="related" type="text/html" href="https://daringfireball.net/linked/2021/09/15/nso-group-imessage-exploit"/>
<id>tag:daringfireball.net,2021:/linked//6.38426</id>
<published>2021-09-15T16:20:04Z</published>
<updated>2021-09-15T16:22:54Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<content type="html" xml:base="https://daringfireball.net/linked/" xml:lang="en">
<![CDATA[ <p>Citizen Lab:</p> <blockquote> <p>In March 2021, we examined the phone of a Saudi activist who has chosen to remain anonymous, and determined that they had been hacked with NSO Group’s Pegasus spyware. During the course of the analysis we obtained an iTunes backup of the device.</p> <p>Recent re-analysis of the backup yielded several files with the “.gif” extension in Library/SMS/Attachments that we determined were sent to the phone immediately before it was hacked with NSO Group’s Pegasus spyware.</p> <p>Because the format of the files matched two types of crashes we had observed on another phone when it was hacked with Pegasus, we suspected that the “.gif” files might contain parts of what we are calling the FORCEDENTRY exploit chain.</p> <p>Citizen Lab forwarded the artifacts to Apple on Tuesday, September 7. On Monday, September 13, Apple confirmed that the files included a zero-day exploit against iOS and MacOS. They designated the FORCEDENTRY exploit CVE-2021-30860, and describe it as “processing a maliciously crafted PDF may lead to arbitrary code execution.”</p> </blockquote> <p>The files with the “.gif” extension weren’t actually GIF files — they were carefully-crafted malformed PSD and PDF files that triggered image processing bugs. What makes attacks like this particularly dastardly is that the victim apparently doesn’t even see anything. It’s invisible.</p> <div> <a title="Permanent link to ‘NSO Group iMessage Zero-Click Exploit Captured in the Wild, Patched by Apple’" href="https://daringfireball.net/linked/2021/09/15/nso-group-imessage-exploit">&nbsp;★&nbsp;</a> </div> ]]>
</content>
</entry>
<entry>
<link rel="alternate" type="text/html" href="https://daringfireball.net/2021/09/iphone_names"/>
<link rel="shorturl" href="http://df4.us/tmz"/>
<id>tag:daringfireball.net,2021://1.38411</id>
<published>2021-09-09T18:40:15Z</published>
<updated>2021-09-10T22:15:45Z</updated>
<author>
<name>John Gruber</name>
<uri>http://daringfireball.net/</uri>
</author>
<summary type="text">I get it: it seems odd that in 10 years we might be awaiting the introduction of the iPhone 23 lineup, but at the moment, I don’t see this changing.</summary>
<content type="html" xml:base="https://daringfireball.net/" xml:lang="en">
<![CDATA[ <p><a href="https://twitter.com/gruber/status/1435292384439508994">I conducted a poll on Twitter this week</a> asking what people think the new iPhones presumably being introduced <a href="https://daringfireball.net/linked/2021/09/07/california-streaming-event">next week</a> will be named. With over 4,600 votes, the results were:</p> <ul> <li>iPhone 13: 70%</li> <li>iPhone 12S: 12%</li> <li>iPhone (no more numbers): 15%</li> <li>Other: 3%</li> </ul> <p>I probably asked a few days too late — there was <a href="https://www.macrumors.com/2021/09/06/iphone-13-pro-max-silicone-cases-leak/">a credible leak</a> purporting to show the packages for “iPhone 13 Pro Max” silicone cases from Apple over the weekend.</p> <p>What intrigued me were the number of folks responding on Twitter who said that while they voted for “iPhone 13” as what they <em>would</em> be named, they <em>wish</em> that Apple would drop the numbers and just go with <em>iPhone</em>, <em>iPhone Mini</em>, <em>iPhone Pro</em>, and <em>iPhone Pro Max</em>, with implicit model years to tell them apart from new models in subsequent years. That’s basically how Apple names its other products — with the notable exception of Apple Watch (see below).</p> <p>But just plain “iPhone” wouldn’t work for iPhones, because iPhones are different. When Apple introduces a new iPad Pro, it <em>replaces</em> the previous iPad Pro. You can’t go into an Apple Store and buy a new 2018 iPad Pro. But you <em>can</em> buy a new iPhone XR from Apple today — a model that <a href="https://daringfireball.net/2018/10/the_iphone_xr">was introduced in 2018</a>. (I’d wait until <a href="https://daringfireball.net/linked/2021/09/07/california-streaming-event">next Tuesday</a> before doing that.) Apple Watch is the only other product that’s sold like iPhones, with previous “series” sticking around for years at lower prices.<sup id="fnr1-2021-09-09"><a href="#fn1-2021-09-09">1</a></sup></p> <p>Apple wants people who are buying new iPhones that were first introduced 2–3 years ago to feel like they’re getting a new iPhone. They should, because they are — they’re great devices at lower prices, and will be supported for years to come. But if the iPhone XR were named “iPhone (2018)”, it’d feel old.</p> <p>I get it: it seems odd that in 10 years we might be awaiting the introduction of the iPhone 23 lineup, but at the moment, I don’t see this changing. <a href="https://www.nfl.com/videos/how-bucs-beat-chiefs-mahomes-in-super-bowl-lv-no-risk-it-no-biscuit">The NFL just keeps counting Super Bowls</a> — at least Apple only used Roman numerals for the X and XS/XR years.</p> <div class="footnotes"> <hr /> <ol> <li id="fn1-2021-09-09"> <p>The Apple Watch numbering scheme is simple: new year, new series, incremented by one. The iPhone numbering scheme is not simple. There was no iPhone 2 — the second iPhone was named iPhone 3G. Thanks to the 3GS, the iPhone 4 was in fact the fourth model year. But then came the other “S” years: 4S, 5S, 6S, XS. And Apple skipped “iPhone 9” entirely. If Apple had stuck to a numbering scheme as simple as Apple Watch’s, next week’s new iPhones would be the iPhones 15.&nbsp;<a href="#fnr1-2021-09-09" class="footnoteBackLink" title="Jump back to footnote 1 in the text.">&#x21A9;&#xFE0E;</a></p> </li> </ol> </div> ]]>
</content>
<title>★ Why iPhone Names Have Numbers and Most Other Apple Product Names Don’t</title>
</entry>
</feed>
<!--  THE END  -->

{
   "version" : "https://jsonfeed.org/version/1.1",
   "title" : "Daring Fireball",
   "home_page_url" : "https://daringfireball.net/",
   "feed_url" : "https://daringfireball.net/feeds/json",
   "authors" : [
      {
         "url" : "https://twitter.com/gruber",
         "name" : "John Gruber"
      }
   ],
   "icon" : "https://daringfireball.net/graphics/apple-touch-icon.png",
   "favicon" : "https://daringfireball.net/graphics/favicon-64.png",
   "items" : [
      {
         "title" : "[Sponsor] Quill — Messaging to Make Your Team Better",
         "date_published" : "2021-09-27T18:31:53-05:00",
         "date_modified" : "2021-09-27T18:31:53-05:00",
         "id" : "https://daringfireball.net/feeds/sponsors/2021/09/quill_messaging_to_make_your_t_1",
         "url" : "https://daringfireball.net/feeds/sponsors/2021/09/quill_messaging_to_make_your_t_1",
         "external_url" : "https://quill.chat/",
         "authors" : [
            {
               "name" : "Daring Fireball Department of Commerce"
            }
         ],
         "content_html" : "\n<p>We love messaging (and most of us grew up using IRC.) It’s our favorite way of collaborating, but not if it’s overwhelming and disorganized. We grew exhausted having to skim thousands of messages every day to keep up, so we built something better. A more deliberate way to chat.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://quill.chat/\">quill.chat/</a></strong></em></p>\n"
      },
      {
         "title" : "★ Why Does the iPhone Still Use Lightning?",
         "date_published" : "2021-09-27T18:27:45Z",
         "date_modified" : "2021-09-27T23:28:04Z",
         "id" : "https://daringfireball.net/2021/09/why_still_lightning",
         "url" : "https://daringfireball.net/2021/09/why_still_lightning",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Chaim Gartenberg, writing for The Verge, “<a href=\"https://www.theverge.com/2021/9/24/22690338/apple-iphone-lightning-ports-convenience-control-usb-c-eu-wireless-charging-mfi-magsafe\">The Lightning Port Isn’t About Convenience; It’s About Control</a>”:</p>\n\n<blockquote>\n  <p>Notably absent from Apple’s argument, though, is the fact that\ncutting out a Lightning port on an iPhone wouldn’t just create\nmore e-waste (if you buy Apple’s logic) or inconvenience its\ncustomers. It also means that Apple would lose out on the revenue\nit makes from every Lightning cable and accessory that works with\nthe iPhone, Apple-made or not — along with the control it has\nover what kinds of hardware does (or doesn’t) get to exist for the\niPhone and which companies get to make them.</p>\n\n<p>Apple’s <a href=\"https://mfi.apple.com/\">MFi program</a> means that if you want to plug anything into\nan iPhone, be it charger or adapter or accessory, you have to go\nthrough Apple. And Apple takes a cut of every one of those\ndevices, too.</p>\n</blockquote>\n\n<p>Gartenberg summarizes a commonly-held theory here: that Apple is sticking with its proprietary Lightning port on iPhones because they profit from MFi peripherals. That it’s a money grab.</p>\n\n<p>I don’t think this is the case at all. Apple is happy to keep the money it earns from MFi, of course. And they’re glad to have control over all iPhone peripherals. But I don’t think there’s serious money in that. It’s loose-change-under-the-couch-cushion revenue by Apple’s astonishingly high standards. How many normal people do you know who ever buy <em>anything</em> that plugs into a Lightning port other than a USB cable? And Apple doesn’t make more money selling their own (admittedly overpriced) Lightning cables to iPhone owners than they do selling their own (also overpriced) USB-C cables to iPad Pro and MacBook owners.</p>\n\n<p>My theory is that Apple carefully weighs the pros and cons for each port on each device it makes, and chooses the technologies for those ports that it thinks makes for the best product for the most people. “<em>What makes sense for the goals of this product that we will ship in three years? And then the subsequent models for the years after that?</em>” Those are the questions Apple product designers ask.</p>\n\n<p>The sub-head on Gartenberg’s piece is “The iPhone doesn’t have USB-C for a reason”. Putting that in the singular does not do justice to the complexity of such decisions. There are numerous reasons that the iPhones 13 still use Lightning — <em>and</em> there are numerous reasons why switching to USB-C would make sense. The pro-USB-C crowd, to me, often comes across as ideological. I’m not accusing Gartenberg of this — though it is his piece with the sub-head claiming there’s “a” singular reason — but many iPhones-should-definitely-use-USB-C proponents argue as though there are no good reasons for the iPhone to continue using Lightning. That’s nonsense.</p>\n\n<p>To be clear, I’m neither pro-Lightning nor pro-USB-C. I see the trade-offs. If the iPhones 13 had switched to USB-C, I wouldn’t have complained. But I didn’t complain about them not switching, either. You’ll note that in none of my reviews of iPad models that have switched from Lightning to USB-C in recent years have I complained about the switch. Apple, to my eyes, has been managing this well. But, if the iPhones 13 <em>had</em> switched to USB-C, you know who <em>would</em> have complained? <em>Hundreds of millions of existing iPhone users</em> who have no interest in replacing the Lightning cables and docks they already own.</p>\n\n<p>When Lightning replaced the old 30-pin iPod connector, starting with the iPhone 5 in 2012, many — I’d say <em>most</em> — existing iPhone users were not happy about it. Many were downright angry. It didn’t matter that the old 30-pin adapter was, compared to Lightning, hideously ungainly, far too large, and technically outdated. (Also, I believe the 30-pin port was impossible or nearly-impossible to make waterproof. The first waterproof models <a href=\"https://support.apple.com/kb/SP743?locale=en_US\">were the iPhones 7 in 2016</a>.) People do not like buying new cables, no matter if they’re “better”. Now, I know what you, someone reading Daring Fireball, might be thinking — <em>I own dozens of USB-C cables already</em> — because you own other products, perhaps several from Apple itself, that do use USB-C. But that’s not true for most iPhone owners around the world. They have Lightning chargers in their kitchens, cars, purses, backpacks, and bedrooms.  All things considered, they do not want to replace any of them, let alone all of them.</p>\n\n<p>In 15 generations of iPhones, Apple has changed the connector once. And that one time was a clear win in every single regard. Changing from Lightning to USB-C is not so clearly an upgrade at all. It’s a sidestep. Note too that when Apple first started changing iPads — <a href=\"https://techcrunch.com/2018/10/30/the-ipad-finally-moves-to-usb-c/\">starting with the iPad Pro in late 2018</a> — from Lightning to USB-C, they didn’t say it was because USB-C is better, period, and certainly not solely for the reason that USB-C is “open”. They said it was to enable iPads Pro to do things that theretofore only PCs and Macs could do, like connecting to external displays. iPhones aren’t meant for that. Or at least aren’t meant for that <em>yet</em> — if ever they are, iPhone peripheral capabilities, including hardware ports, will change.</p>\n\n<p>If you’re on team “Lightning is nothing but a money grab”, you should explain why, for inductive (a.k.a. wireless) charging, iPhones have supported industry-standard Qi from day one. Or why iPads have been steadily moving from Lightning to USB-C. Or why Apple was the first laptop maker to go all-in on USB-C, literally <a href=\"https://www.macworld.com/article/225278/review-the-new-12-inch-macbook-is-a-laptop-without-an-ecosystem.html\">making a laptop with no ports other than a single USB-C port</a> and a headphone jack.</p>\n\n<p>Speaking of headphone jacks, my theory is the same with those. Apple’s not “against” headphone jacks. They’ve begun steadily removing them from new products only when they deem doing so the best trade-off. The <a href=\"https://support.apple.com/kb/SP850\">new iPad Mini</a> has no headphone jack; the <a href=\"https://support.apple.com/kb/SP849\">new regular iPad</a> that debuted alongside it does. That’s not ideal, but it’s not incoherent. They are different products for different users with different needs and different priorities. These decisions require nuance. “<em>Apple’s just trying to force everyone to buy $160 AirPods</em>” is not a nuanced argument. Is it a consideration that removing the headphone jack from more products each year might steer more customers toward their first AirPods purchase? Sure. But it’s not like there aren’t other brands of wireless headphones.</p>\n\n<p>To say that there’s <em>a</em> reason that the iPhones 13 still use Lightning, any singular reason, is facile.</p>\n\n\n\n    "
      },
      {
         "title" : "Yours Truly on The HourTime Show",
         "date_published" : "2021-09-27T17:25:03Z",
         "date_modified" : "2021-09-27T17:25:03Z",
         "id" : "https://daringfireball.net/linked/2021/09/27/the-hourtime-show",
         "url" : "https://daringfireball.net/linked/2021/09/27/the-hourtime-show",
         "external_url" : "https://anchor.fm/the-hourtime-show/episodes/Why-Its-So-Hard-to-Buy-a-Rolex-Gruber-Guest-Appearance-e17tji8",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>I had the distinct pleasure of a guest appearance on this week’s episode of The HourTime Show, a watch nerd podcast from the gang at WristWatchReview — John Biggs, Victor Marks, and Nicholas De Leon. The topic: why it’s <a href=\"https://www.wristwatchreview.com/rolex-claims-the-supply-shortage-is-not-planned-unconvincingly/\">so crazy hard</a> to buy a new Rolex.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://anchor.fm/the-hourtime-show/episodes/Why-Its-So-Hard-to-Buy-a-Rolex-Gruber-Guest-Appearance-e17tji8\">anchor.fm/the-hourtime-show/episodes/Why-Its-So-Hard-to-Buy…</a></strong></em></p>\n"
      },
      {
         "title" : "Wil Shipley Joins Apple",
         "date_published" : "2021-09-27T17:19:00Z",
         "date_modified" : "2021-09-27T17:19:00Z",
         "id" : "https://daringfireball.net/linked/2021/09/27/shipley-apple",
         "url" : "https://daringfireball.net/linked/2021/09/27/shipley-apple",
         "external_url" : "https://twitter.com/wilshipley/status/1442528831689007112",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>On the one hand, I did not see that coming. On the other hand is <a href=\"https://twitter.com/atomicbird/status/499576229734150144\">this apt observation from Tom Harrington</a>:</p>\n\n<blockquote>\n  <p>How to make technical contacts at Apple:</p>\n\n<ol>\n<li>Meet any developer who knows what they’re doing.</li>\n<li>Wait.</li>\n<li>They now work for Apple.</li>\n</ol>\n</blockquote>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://twitter.com/wilshipley/status/1442528831689007112\">twitter.com/wilshipley/status/1442528831689007112</a></strong></em></p>\n"
      },
      {
         "title" : "If Unlock With Apple Watch Isn’t Working on Your iPhone 13",
         "date_published" : "2021-09-27T14:43:23Z",
         "date_modified" : "2021-09-27T14:44:44Z",
         "id" : "https://daringfireball.net/linked/2021/09/27/apple-watch-unlock-iphone-13",
         "url" : "https://daringfireball.net/linked/2021/09/27/apple-watch-unlock-iphone-13",
         "external_url" : "https://support.apple.com/en-us/HT212828",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Apple support document acknowledges a problem a lot of iPhone 13 users are running into:</p>\n\n<blockquote>\n  <p>Apple has identified an issue where <a href=\"https://support.apple.com/kb/HT212208\">Unlock with Apple Watch</a>\nmay not work with iPhone 13 devices. You might see “Unable to\nCommunicate with Apple Watch” if you try to unlock your iPhone\nwhile wearing a face mask, or you might not be able to set up\nUnlock with Apple Watch.</p>\n\n<p>This issue will be fixed in an upcoming software update. Until the\nupdate is available, you can turn off Unlock with Apple Watch and\nuse your passcode to unlock your iPhone 13.</p>\n</blockquote>\n\n<p>I haven’t seen this issue, but I sympathize with those of you who’ve been hit by it. “Unlock With Apple Watch” almost completely mitigates the annoyance of using an iPhone with Face ID while wearing a mask.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://support.apple.com/en-us/HT212828\">support.apple.com/en-us/HT212828</a></strong></em></p>\n"
      },
      {
         "title" : "Retool",
         "date_published" : "2021-09-26T21:29:30Z",
         "date_modified" : "2021-09-26T21:30:13Z",
         "id" : "https://daringfireball.net/linked/2021/09/26/retool",
         "url" : "https://daringfireball.net/linked/2021/09/26/retool",
         "external_url" : "https://retool.com/?utm_source=sponsor&utm_medium=newsletter&utm_campaign=daringfireball",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>My thanks to Retool for sponsoring last week at DF. Retool is a new approach to programming for the modern web: they’ve unified the ease of visual programming with the power and flexibility of real code. Drag and drop a form together, and have it <code>POST</code> back to your API in minutes. Deploy instantly with access controls and audit logs. It’s akin to a HyperCard or Visual Basic for the modern web.</p>\n\n<p>Allbirds uses Retool to measure billboard efficacy. Amazon uses Retool to handle GDPR requests. You, too, can use it to build business-critical applications fast.</p>\n\n<p>Check out their demo video to see how easy it is to build something serious and useful — quickly and intuitively. It’s easy to explore on your own <em>and</em> they have <a href=\"https://docs.retool.com/docs\">good docs</a> and guided videos. <a href=\"https://retool.com/?utm_source=sponsor&amp;utm_medium=newsletter&amp;utm_campaign=daringfireball\">Start building for free today</a>.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://retool.com/?utm_source=sponsor&utm_medium=newsletter&utm_campaign=daringfireball\">retool.com/?utm_source=sponsor&utm_medium=newsletter&utm…</a></strong></em></p>\n"
      },
      {
         "title" : "Arun Maini’s Battery Life Stress Test for the New iPhones 13",
         "date_published" : "2021-09-25T21:00:30Z",
         "date_modified" : "2021-09-25T21:00:31Z",
         "id" : "https://daringfireball.net/linked/2021/09/25/arun-maini-iphone-13-battery-stress-test",
         "url" : "https://daringfireball.net/linked/2021/09/25/arun-maini-iphone-13-battery-stress-test",
         "external_url" : "https://www.youtube.com/watch?v=IQQCoJiZj8w",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>YouTuber Arun “Mrwhosetheboss” Maini’s full battery life drain test of the iPhone 13 Pro Max, iPhone 13 Pro, iPhone 13, iPhone 13 Mini, iPhone 12, iPhone 11, and iPhone SE. Interesting results that jibe with Apple’s claims about the improvements to battery life in the iPhones 13.</p>\n\n<p><a href=\"https://twitter.com/greengart/status/1441426882893914112\">Via Avi Greengart</a>, who observes the most impressive result:</p>\n\n<blockquote>\n  <p>It’s worth watching Arun’s whole video, but the iPhone 13 mini\nhandily beats last year’s full-sized iPhone 12 on battery life,\nmaking it an easy recommendation for anyone with human-sized\nhands. The entire iPhone 13 line has genuinely good to\nextraordinary battery life.</p>\n</blockquote>\n\n<p>The iPhone 13 Mini has longer battery life than last year’s regular iPhone 12. That’s a game-changer for those who want the Mini size.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.youtube.com/watch?v=IQQCoJiZj8w\">youtube.com/watch?v=IQQCoJiZj8w</a></strong></em></p>\n"
      },
      {
         "title" : "Try Safari 15 Before You Buy, With Safari Technology Preview",
         "date_published" : "2021-09-25T20:23:01Z",
         "date_modified" : "2021-09-25T20:23:02Z",
         "id" : "https://daringfireball.net/linked/2021/09/25/try-safari-15-tech-preview",
         "url" : "https://daringfireball.net/linked/2021/09/25/try-safari-15-tech-preview",
         "external_url" : "https://developer.apple.com/safari/technology-preview/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>MacOS 12 Monterey is not out yet — and, I hope, won’t ship until after a few more weeks of much-needed bug fixes — but Safari 15 for MacOS 11 Big Sur <a href=\"https://arstechnica.com/gadgets/2021/09/apple-rolls-major-safari-redesign-out-to-macs-ahead-of-monterey-release/\">shipped last week</a>. I strongly recommend <em>not</em> upgrading, unless you’ve already tried the new tab design and like it, or at least feel ambivalent about it. Updates like this are why I always <a href=\"/misc/2021/09/software-update-auto-checkbox.png\">turn off “Automatically keep my Mac up to date”</a> in System Preferences → Software Update.</p>\n\n<p>The sole reason I recommend not upgrading to Safari 15 is the new tab bar design. You can easily try it out for yourself, though, without upgrading to Safari 15 or installing the MacOS 12 betas. Safari Technology Preview is a <em>separate</em> version of Safari you can easily install next to regular Safari. Typically it’s used by web developers to test in-progress changes to WebKit, but right now it’s more useful as a way to preview the new Safari 15 tab design. It’s easy to install and easy to uninstall. You can even set it as your default web browser while testing in System Preferences: General.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://developer.apple.com/safari/technology-preview/\">developer.apple.com/safari/technology-preview/</a></strong></em></p>\n"
      },
      {
         "title" : "Daring Fireball Weekly Sponsorships for Q4",
         "date_published" : "2021-09-24T23:30:00Z",
         "date_modified" : "2021-09-25T17:00:27Z",
         "id" : "https://daringfireball.net/linked/2021/09/24/df-sponsorships-q4",
         "url" : "https://daringfireball.net/linked/2021/09/24/df-sponsorships-q4",
         "external_url" : "https://daringfireball.net/feeds/sponsors/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Sponsorships have been selling briskly this year, but I’ve only just now opened spots for the October-December quarter. <s><em>Plus</em>, a last-minute change has opened up next week’s spot, starting this coming Monday.</s></p>\n\n<p>One sponsor per week, with a sponsor-written entry in the RSS feed to start the week, a thank-you post right on the homepage from me at the end, and the one and only graphic ad on every page of the site all week long. No tracking or other privacy-invasive bullshit. Just plain honest ads. That’s not new — that’s the way the ads on DF have <a href=\"https://daringfireball.net/2004/09/sponsor_this\">always been</a>. My best argument that they work: <a href=\"https://daringfireball.net/feeds/sponsors/archive\">the number of repeat companies in the sponsor archive list</a>.</p>\n\n<p>So if you’ve got a product or service you’d like to promote to DF’s discerning audience, <a href=\"mailto:sponsors@daringfireball.net?subject=Feed%20Sponsorship\">I’d love to have you as a sponsor</a>. <s>And if you’re ready to grab next week’s opening, let’s go — should be another good week.</s></p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://daringfireball.net/feeds/sponsors/\">daringfireball.net/feeds/sponsors/</a></strong></em></p>\n"
      },
      {
         "title" : "‘Float’",
         "date_published" : "2021-09-24T23:29:00Z",
         "date_modified" : "2021-09-25T17:14:42Z",
         "id" : "https://daringfireball.net/linked/2021/09/24/float",
         "url" : "https://daringfireball.net/linked/2021/09/24/float",
         "external_url" : "https://www.youtube.com/watch?v=H8qFTgcRV6w",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Aundre Larrow, announcing his directorial debut:</p>\n\n<blockquote>\n  <p>Shot on the new iPhone 13 Pro, <em>Float</em> is a short film about the\njourney that a father and daughter take together.</p>\n</blockquote>\n\n<p>If this doesn’t move you, you’re not hooked up right. Good god, what a powerful, lovely, beautiful short film. Headphones and full screen — this deserves your attention. I <a href=\"https://daringfireball.net/2021/09/the_iphones_13#cinematic_mode\">take it back</a>, Cinematic mode — <a href=\"https://twitter.com/aundrelarrow/status/1441025854977417224\">which Larrow used to shoot this</a> — is no gimmick at all.</p>\n\n<p>This is just astonishing. Remember Aundre Larrow’s name.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.youtube.com/watch?v=H8qFTgcRV6w\">youtube.com/watch?v=H8qFTgcRV6w</a></strong></em></p>\n"
      },
      {
         "title" : "iPhone Day Is Still a Thing",
         "date_published" : "2021-09-24T23:06:43Z",
         "date_modified" : "2021-09-27T23:08:50Z",
         "id" : "https://daringfireball.net/linked/2021/09/24/iphone-day",
         "url" : "https://daringfireball.net/linked/2021/09/24/iphone-day",
         "external_url" : "https://vimeo.com/613966202",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>I shot this video while walking past the Philly Apple Store at 2 pm. The line went most of the way down the block. I’ll bet the line was longer than it would have been without COVID restrictions, but still — this is the 15th generation of iPhones and people are <a href=\"https://daringfireball.net/linked/2017/11/03/iphone-x-campout\">still</a> lining up to buy them on the day they’re available. And how many <em>more</em> people had them delivered today, waking up early a week ago to preorder the moment the online store came online? People love the iPhone. If you look at it solely as a technology product you’re missing the biggest part of the iPhone story. iPhone Day is a de facto annual holiday for untold millions of people <a href=\"https://www.apple.com/newsroom/2021/09/iphone-13-lineup-new-ipad-mini-and-ninth-generation-ipad-arrive-worldwide/\">around the world</a>.</p>\n\n<p>That’s not true of any other product in the world.</p>\n\n<div style=\"padding:56.25% 0 0 0;position:relative;\"><iframe src=\"https://player.vimeo.com/video/613966202?h=444a7a0f19&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479\" frameborder=\"0\" allow=\"autoplay; fullscreen; picture-in-picture\" allowfullscreen style=\"position:absolute;top:0;left:0;width:100%;height:100%;\" title=\"iPhone Day 2021, Philadelphia\"></iframe></div>\n\n<script src=\"https://player.vimeo.com/api/player.js\"></script>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://vimeo.com/613966202\">vimeo.com/613966202</a></strong></em></p>\n"
      },
      {
         "title" : "Apple’s iOS Changes Are Hurting Facebook’s Ad Business",
         "date_published" : "2021-09-24T22:01:34Z",
         "date_modified" : "2021-09-24T22:01:34Z",
         "id" : "https://daringfireball.net/linked/2021/09/24/apple-facebook-kantrowitz",
         "url" : "https://daringfireball.net/linked/2021/09/24/apple-facebook-kantrowitz",
         "external_url" : "https://www.cnbc.com/2021/09/24/apples-ios-changes-hurt-facebooks-ad-business.html",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Alex Kantrowitz, writing for CNBC:</p>\n\n<blockquote>\n  <p>“Just completely running blind” is how Aaron Paul, a performance\nFacebook marketer, described it. Paul said his company, Carousel,\nmoved from spending millions of dollars each day on Facebook to a\nfew hundred thousand dollars. Before the iOS changes, Facebook\ngenerated 80% of the traffic Carousel sent to its product pages.\nNow it accounts for 20%.</p>\n\n<p>Apple’s iOS changes may lead to irreparable harm to Facebook’s ad\nbusiness. This moment has demonstrated to Paul and his fellow\nperformance buyers that relying on one channel (albeit a very\neffective one) is risky. So they’re looking to diversify their ad\nspend. Paul said he’s moved his ad budget elsewhere, including\n“<a href=\"https://www.cnbc.com/quotes/SNAP\">Snapchat</a> and TikTok, but also silent killers like email.” On\n<a href=\"https://www.cnbc.com/quotes/TWTR\">Twitter</a>, Facebook marketers discussing Apple’s changes\n<a href=\"https://twitter.com/search?q=https%3A%2F%2Ftwitter.com%2Fsoundslikecanoe%2Fstatus%2F1440117176132935683&amp;src=typed_query\">almost unanimously agreed</a> they needed to follow suit.</p>\n</blockquote>\n\n<p>🎻.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.cnbc.com/2021/09/24/apples-ios-changes-hurt-facebooks-ad-business.html\">cnbc.com/2021/09/24/apples-ios-changes-hurt-facebooks-ad…</a></strong></em></p>\n"
      },
      {
         "title" : "Another Sign of Microsoft Establishing ‘Surface’ as a Standalone Brand",
         "date_published" : "2021-09-24T22:00:00Z",
         "date_modified" : "2021-09-25T20:10:42Z",
         "id" : "https://daringfireball.net/linked/2021/09/24/surface-brand",
         "url" : "https://daringfireball.net/linked/2021/09/24/surface-brand",
         "external_url" : "https://surface.com/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>To <a href=\"https://daringfireball.net/linked/2021/09/23/surface-event-highlights\">my point yesterday</a> about Microsoft establishing “Surface” as a brandname, sans “Microsoft” as a prefix — the headline on the Surface homepage (which redirects from surface.com): “New laptops from Surface, now with Windows 11”.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://surface.com/\">surface.com/</a></strong></em></p>\n"
      },
      {
         "title" : "App Store Release Notes of the Week: Poolsuite FM",
         "date_published" : "2021-09-24T17:49:43Z",
         "date_modified" : "2021-09-24T17:49:44Z",
         "id" : "https://daringfireball.net/linked/2021/09/24/poolsuite-fm-release-notes",
         "url" : "https://daringfireball.net/linked/2021/09/24/poolsuite-fm-release-notes",
         "external_url" : "https://twitter.com/gruber/status/1441423424337764362",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>This is the most joyful way of saying “We’re sorry our iOS 15 compatibility update was a few days late” I can imagine. What a fun app.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://twitter.com/gruber/status/1441423424337764362\">twitter.com/gruber/status/1441423424337764362</a></strong></em></p>\n"
      },
      {
         "title" : "Monotype Acquires Hoefler&Co.",
         "date_published" : "2021-09-24T15:51:05Z",
         "date_modified" : "2021-09-26T19:13:56Z",
         "id" : "https://daringfireball.net/linked/2021/09/24/monotype-hoefler",
         "url" : "https://daringfireball.net/linked/2021/09/24/monotype-hoefler",
         "external_url" : "https://www.typography.com/blog/monotype-acquires-hoeflerco",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Jonathan Hoefler:</p>\n\n<blockquote>\n  <p>Nothing’s changing at typography.com, where you’ll still find all\n1,113 fonts in the Hoefler&amp;Co library, as well as the\ncloud.typography webfont service, and all the other resources\nwe’ve created for designers and brands. The H&amp;Co team is staying\nin place, too, and there are yet more typefaces from us that you\ncan look forward to seeing soon. […]</p>\n\n<p>In the meantime, I’ll be stepping down from my role in the\ncompany, to finally make the time to recharge, reflect, and\nexplore some new ideas. In these past few years, <a href=\"https://www.typography.com/blog/abstract-typography-episode\">participating in\na documentary</a> and using typography to help <a href=\"https://www.typography.com/blog/biden-fonts\">elect a\npresident</a> have been potent reminders of just how many ways\nthere are for type to make a difference, and just how many people\nare moved by the splendor of typography.</p>\n</blockquote>\n\n<p>I’d need 144-point type to express my surprise at this announcement.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.typography.com/blog/monotype-acquires-hoeflerco\">typography.com/blog/monotype-acquires-hoeflerco</a></strong></em></p>\n"
      },
      {
         "title" : "iPhone 13 Pro Works, But Fits Poorly With MagSafe Duo Charger",
         "date_published" : "2021-09-24T15:05:08Z",
         "date_modified" : "2021-09-24T15:05:08Z",
         "id" : "https://daringfireball.net/linked/2021/09/24/iphone-13-pro-magsafe-duo",
         "url" : "https://daringfireball.net/linked/2021/09/24/iphone-13-pro-magsafe-duo",
         "external_url" : "https://twitter.com/MKBHD/status/1441086122839339015",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Awkward.</p>\n\n<p><em>(Remembers that the MagSafe Duo Charger costs $130.)</em></p>\n\n<p><em>Really</em> awkward.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://twitter.com/MKBHD/status/1441086122839339015\">twitter.com/MKBHD/status/1441086122839339015</a></strong></em></p>\n"
      },
      {
         "title" : "My Advice on How to Set Up a New iPhone or iPad: Quick Start Device-to-Device Transfer",
         "date_published" : "2021-09-24T05:14:54Z",
         "date_modified" : "2021-09-25T15:11:57Z",
         "id" : "https://daringfireball.net/linked/2021/09/24/how-to-set-up-a-new-iphone-or-ipad",
         "url" : "https://daringfireball.net/linked/2021/09/24/how-to-set-up-a-new-iphone-or-ipad",
         "external_url" : "https://support.apple.com/en-us/HT210216",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>A bunch of you are probably getting new iPhones (and iPads) today. As someone who’s set up 5 new devices in the last week, my advice is to restore a new iPhone with the Quick Start device-to-device transfer, not iCloud backup. Don’t worry if it says it might take a little longer this way, it’s worth it. Get a cup of coffee or a bite to eat. A watched pot never boils; a watched transfer never finishes.</p>\n\n<p>Device-to-device is better because it moves over <em>all</em> your login credentials. When you restore from an iCloud backup, you wind up logged out of a <em>lot</em> of apps on the new device. When you restore device-to-device, almost everything moves over. I know there are <a href=\"https://twitter.com/renefouquet/status/1441259286177325063\">exceptions</a>, but I don’t think I bounced into a single app that didn’t keep me fully logged in this week. If you tried device-to-device a few years ago and found it lacking, try it again now — Apple has improved this process every year since it debuted. Worst case scenario, you can always start over and use iCloud backup.</p>\n\n<p>Also, you do not need to unpair your Apple Watch from your old iPhone using this method. You can just wear your watch the whole time. When the transfer is complete, the new iPhone will prompt you, asking if you want to move your watch to the new iPhone. Your mileage may vary but it just worked for me.</p>\n\n<p><a href=\"https://twitter.com/gruber/status/1441255208558997506\">I posted this on Twitter tonight</a>, and realized I should post about this here too. The Twitter thread has a bunch of Q&amp;A’s about specific apps, like authentication tokens in Authy (they transfer fine).</p>\n\n<p><strong>Update, 25 September 2021:</strong> Lots of positive feedback from readers who took my advice. Perfect? No. But I’m more convinced than ever that device-to-device transfer is the way to go. Apple has done a lot of work, year after year, to keep making this migration experience better, faster, simpler, more complete, and more reliable. I see it firsthand, setting up multiple new iOS devices a year. The team behind this doesn’t get enough thanks, so let me say it: thank you.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://support.apple.com/en-us/HT210216\">support.apple.com/en-us/HT210216</a></strong></em></p>\n"
      },
      {
         "title" : "Om Malik on the New iPad Mini",
         "date_published" : "2021-09-23T23:49:28Z",
         "date_modified" : "2021-09-24T14:31:46Z",
         "id" : "https://daringfireball.net/linked/2021/09/23/om-malik-ipad-mini",
         "url" : "https://daringfireball.net/linked/2021/09/23/om-malik-ipad-mini",
         "external_url" : "https://om.co/2021/09/22/the-ipad-mini-2021-review/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Om Malik:</p>\n\n<blockquote>\n  <p>The best way to extract the most out of the smallest iPad is to\nthink of it as a device enhanced by non-keyboard input methods — Scribble with Pencil, snapping photos with the cameras, or\nusing Siri/voice input. The improved “Scribble” allows you to\nmake notes, do quick searches, and even find directions. It is a\nvery addictive way to use the iPad, especially in the smaller\nsize. […]</p>\n\n<p>The more I use the device, the more I realize that most computing\nhas been defined by a singular idea of work and productivity.\nMobile devices have and will continue to redefine our work. In the\npast, most of the computing involved being in the office. Now,\nnon-office tasks have access to computing resources and thus offer\nan opportunity to make them more productive. Devices like the iPad\nare about making non-office work a bit more productive. Whether it\nis doctors, field engineers, or delivery drivers, devices such as\nthe iPad in general and iPad Mini, in particular, could help\nchange the very notion of productivity.</p>\n</blockquote>\n\n<p>What makes Om’s perspective interesting to me is that he switched to an iPad Pro as his main computer a few years back, and loves it. The iPad Mini isn’t an alternative to those sort of use cases — but as he points out, there are so many things people do with “computers” today that just weren’t imagined even a decade ago.</p>\n\n<p>I’m sort of the anti-Om in this regard. I have a 2018 iPad Pro that I generally keep in my kitchen, connected to a Magic Keyboard. <a href=\"https://daringfireball.net/2020/04/the_ipad_magic_keyboard\">Ever since the Magic Keyboard came out</a> (with trackpad support and good keyboard shortcut support in iPadOS), I’ve found the iPad Pro <em>much</em> more useful for my work. But nowhere near as useful as a Mac. I’m not arguing that a MacBook is better than an iPad for work. I’m just saying MacOS works better for me. Not even close. Getting in the flow on my Mac, I feel 10 times more productive than I ever do on my iPad Pro. But the iPad Pro with Magic Keyboard is good enough that I now suspect it leads me to punt around in the kitchen drinking coffee <em>much</em> longer than I should at the start of my workdays. I like an iPad for reading the news at the start of the day, but I might be better served with a more limited iPad Mini than a significantly more useful iPad Pro with Magic Keyboard, just because it’d push me to get to my office and sit my ass in front of my real work machine.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://om.co/2021/09/22/the-ipad-mini-2021-review/\">om.co/2021/09/22/the-ipad-mini-2021-review/</a></strong></em></p>\n"
      },
      {
         "title" : "The Microsoft Event Had In-Person Hands-On Time With Products",
         "date_published" : "2021-09-23T23:41:48Z",
         "date_modified" : "2021-09-24T05:29:48Z",
         "id" : "https://daringfireball.net/linked/2021/09/23/microsoft-event-was-in-person",
         "url" : "https://daringfireball.net/linked/2021/09/23/microsoft-event-was-in-person",
         "external_url" : "https://twitter.com/caro_milanesi/status/1440709608608202756",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Carolina Milanesi, on Twitter:</p>\n\n<blockquote>\n  <p>I had the opportunity to see the new @surface devices live … and I\nam so glad I did.</p>\n\n<p>Holding #SurfaceDuo in my hand, seeing the clever case that\nsecures the #SurfacePen that looks like a finish rather than a\ncase not adding any thickness, the fluidity of the screen and\nthe clever gaming controls…. Very much looking forward to giving\nit a spin!</p>\n</blockquote>\n\n<p>Amen to this enthusiasm for seeing the product introduction live. I get it why Apple did not hold an in-person press event last week — iPhone events are <em>huge</em>, and while I think small events can safely be held in person now, there’s no practical way to shrink the iPhone event.</p>\n\n<p>I miss having hands-on time with new devices as soon as keynotes end. You pick up on things immediately: that something is heavier or lighter than you expected. That certain colors or finishes look different. Remember the Jet Black iPhone 7? You <em>had</em> to see it in person to understand how it looked. And I miss in-person briefings, both official ones and unofficial. In-person communication simply cannot be beaten for conveying subtlety.</p>\n\n<p>Product reviews are hampered too. With in-person Apple events, most reviewers get kit in the hours after the keynote ends. With virtual Apple events, the kit ships for delivery the next day. An extra day makes a big difference when the review embargo drops just one week after the event.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://twitter.com/caro_milanesi/status/1440709608608202756\">twitter.com/caro_milanesi/status/1440709608608202756</a></strong></em></p>\n"
      },
      {
         "title" : "Highlights From Microsoft’s Fall Surface Event",
         "date_published" : "2021-09-23T23:26:05Z",
         "date_modified" : "2021-09-24T06:17:35Z",
         "id" : "https://daringfireball.net/linked/2021/09/23/surface-event-highlights",
         "url" : "https://daringfireball.net/linked/2021/09/23/surface-event-highlights",
         "external_url" : "https://www.theverge.com/2021/9/22/22684950/microsoft-surface-event-biggest-announcements-pro-8-duo-studio-laptop",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Nice supercut video from The Verge squeezing Microsoft’s Surface event yesterday into eight minutes. A few thoughts:</p>\n\n<p>It seems like Microsoft is letting the Surface division stand on its own, brand-wise. They’re not distancing themselves from Microsoft in any way, but branding-wise they’re just letting the products be the “Surface Whatever”, not the “Microsoft Surface Whatever”. There’s even a moment in the event, regarding the folding Duo 2 phone, when a guy says it has “the most precise and reliable hinge mechanism ever engineered at Surface”. I.e. that it was “Surface” who engineered that hinge, not “Microsoft”. I think Surface works as a Microsoft sub-brand like that.</p>\n\n<p>Speaking of the Surface Duo 2 — their folding phone with two screens — they’re now just calling it what they should have called it all along: a phone. It’s a very interesting and unique form factor, but it’s a big folding phone, not a small folding tablet. It supposedly has real cameras this time, too. Starting price: $1,500.</p>\n\n<p>The new Surface Laptop Studio looks really dumb to me. I don’t understand why one would ever want to use it in either of the new folding positions. I guess maybe if you really want to draw on it, you might want to fold it flat, but if you really want to draw that much, why not buy the Surface Pro 8 that detaches from the keyboard? This design <a href=\"https://www.theverge.com/2021/9/23/22688432/microsoft-surface-laptop-studio-book-3-specs-step-backwards\">just seems dumb</a>.</p>\n\n<p>The Surface Slim Pen 2 introduces haptic feedback, to simulate the feel of a pen on paper. I love stuff like that.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.theverge.com/2021/9/22/22684950/microsoft-surface-event-biggest-announcements-pro-8-duo-studio-laptop\">theverge.com/2021/9/22/22684950/microsoft-surface-event…</a></strong></em></p>\n"
      },
      {
         "title" : "Apple Watch Series 7 Supports 60.5GHz Wireless Data Transfer, Perhaps Only for Apple’s Internal Use",
         "date_published" : "2021-09-23T22:13:08Z",
         "date_modified" : "2021-09-24T05:04:52Z",
         "id" : "https://daringfireball.net/linked/2021/09/23/series-7-wireless-data-transfer",
         "url" : "https://daringfireball.net/linked/2021/09/23/series-7-wireless-data-transfer",
         "external_url" : "https://www.macrumors.com/2021/09/23/apple-watch-60-5-ghz-wireless-data-transfer/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Joe Rossignol, reporting for MacRumors:</p>\n\n<blockquote>\n  <p>Apple Watch Series 7 models are equipped with a new module that\nenables 60.5GHz wireless data transfer, according to <a href=\"https://www.scribd.com/document/527108597/Apple-Watch-Series-7-FCC-Filing\">FCC\nfilings</a> viewed by MacRumors, but this functionality may be\nreserved for Apple’s internal use only for now.</p>\n\n<p>The filings indicate that the 60.5GHz module is only activated\nwhen the Apple Watch is placed on a proprietary magnetic dock with\na corresponding 60.5GHz module, but this dock will likely be\nreserved for use by Apple employees. For example, it’s possible\nthat Apple Stores might use the dock to wirelessly restore an\nApple Watch, and if so, it will be interesting to see if Series 7\nmodels still have a hidden diagnostic port for wired connectivity.</p>\n</blockquote>\n\n<p>This is a little interesting in and of itself. But if you look at the long-term trend, it’s a sign that Apple — along with the rest of the industry — is moving toward wireless technology for both charging <em>and</em> data transfer. Apple Watch exemplifies that — it’s <em>never</em> had a port, either for charging or data. There’s a diagnostic port hidden inside the bottom channel for the watch strap, but those <em>diagnostics</em> are neither charging nor data.</p>\n\n<p>It’s long been my guess that iPhone is never going to support USB-C. I think it’s Apple’s intention to go straight from Lightning to wireless/inductive, with no “port”. Portless is the future for all devices. Yet the product design geniuses at the European Commission want to mandate all devices have one specific port in 2024 and indefinitely thereafter — a port that by that time <a href=\"https://en.wikipedia.org/wiki/USB-C\">will already be 10 years old</a>.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.macrumors.com/2021/09/23/apple-watch-60-5-ghz-wireless-data-transfer/\">macrumors.com/2021/09/23/apple-watch-60-5-ghz-wireless-data…</a></strong></em></p>\n"
      },
      {
         "title" : "European Commission Unveils Long-Awaited Stupid Proposal to Mandate USB-C on All Cell Phones and Devices",
         "date_published" : "2021-09-23T21:41:34Z",
         "date_modified" : "2021-09-24T01:09:01Z",
         "id" : "https://daringfireball.net/linked/2021/09/23/eu-usbc-mandate",
         "url" : "https://daringfireball.net/linked/2021/09/23/eu-usbc-mandate",
         "external_url" : "https://www.nytimes.com/2021/09/23/business/european-union-apple-charging-port.html",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Elian Peltier, reporting for The New York Times:</p>\n\n<blockquote>\n  <p>The European Union unveiled plans on Thursday to make USB-C\nconnectors the standard charging port for all smartphones, tablets\nand other electronic devices sold across the bloc, an initiative\nthat it says will reduce environmental waste but that is likely to\nhit Apple the hardest.</p>\n\n<p>The move would represent a long-awaited yet aggressive step into\nproduct-making decisions by the European Commission, the bloc’s\nexecutive arm. Apple, whose iPhones are equipped with a different\nport, has long opposed the plan, arguing that it would stifle\ninnovation and lead to more electronic waste as all current\nchargers that are not USB-C would become obsolete. […]</p>\n\n<p>The <a href=\"https://ec.europa.eu/commission/presscorner/detail/en/ip_21_4613\">new legislation</a> is likely to come into effect in 2024\nbecause it first needs to be approved by the European Parliament\nand then adopted by manufacturers. Besides phones, it would apply\nto cameras, headphones, portable speakers and video game consoles.</p>\n</blockquote>\n\n<p><a href=\"https://twitter.com/benedictevans/status/1441009296540676096\">Benedict Evans</a>:</p>\n\n<blockquote>\n  <p>This is a profoundly stupid way to approach product design and\nstandardisation. What happens in 5 years when someone wants to use\na better connector? What if they’d picked USB 3 five years ago?</p>\n</blockquote>\n\n<p>How stupid? This stupid:</p>\n\n<blockquote>\n  <p>But Apple has also argued that if the European Union had imposed a\ncommon charger in 2009, it would have restricted innovation that\nled to USB-C and Lightning connectors. In a statement, Apple said\nthat although it welcomed the European Commission’s commitment to\nprotecting the environment, it favored a solution that left the\ndevice side of the charging interface open for innovation.</p>\n\n<p>Mr. Breton said on Thursday that he was familiar with Apple’s\nconcerns. “Every time we try to put a proposal, such companies\nstart to say, ‘It will be against innovation,’” he said.</p>\n\n<p>“It’s not at all against innovation. It’s not against anyone,” he\nadded. “It’s for European consumers.”</p>\n\n<p>Mr. Breton said manufacturers, including Apple, could choose to\noffer two charging ports on their devices if they wanted to keep a\nnon-USB-C connector.</p>\n</blockquote>\n\n<p>Two charging ports on the same phone, what an elegant idea. This is like a parody of overzealous regulation of something that is not in need of any regulation at all. Why not mandate that all phones, tablets, and cameras have to run the same operating system, too? Oh, you say, it’s only about reducing waste? Why not mandate that all phones must be the same size and shape, so that they’re all compatible with the exact same cases? Great idea.</p>\n\n<p>These E.U. meddlers have indeed been clamoring for this legislation since 2009 — Apple didn’t pick that date out of the air. At the time, iPhones used 30-pin iPod USB 1 adapters and most other phones used adapters like Micro-USB and (gag) Mini-USB. You don’t have to be a computer engineer to look back at your lifetime and realize that computer plugs and adapters keep getting smaller and better. Do they really think no one is going to come up with an adapter better than USB-C? Ever?</p>\n\n<p>And don’t even start with any sort of argument that legislation like this won’t impede progress, but will instead force the industry to work together via committee to agree upon new better standards in a prompt fashion. Almost everything that goes through such committees takes <em>years</em> longer than one company can do on its own, and comes out worse — often far worse. <a href=\"https://en.wikipedia.org/wiki/USB#Receptacle_(socket)_identification\">Look at all the horrendously shitty USB plugs</a> the USB consortium has come up with over the years.</p>\n\n<p>And people in the E.U. wonder why England wanted out, and why nearly all the major tech companies are from the U.S. and Asia.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.nytimes.com/2021/09/23/business/european-union-apple-charging-port.html\">nytimes.com/2021/09/23/business/european-union-apple…</a></strong></em></p>\n"
      },
      {
         "title" : "Austin Mann’s iPhone 13 Pro Camera Review: Tanzania",
         "date_published" : "2021-09-23T21:10:47Z",
         "date_modified" : "2021-09-23T21:12:10Z",
         "id" : "https://daringfireball.net/linked/2021/09/23/mann-mckay-iphone-13-tanzania",
         "url" : "https://daringfireball.net/linked/2021/09/23/mann-mckay-iphone-13-tanzania",
         "external_url" : "https://austinmann.com/trek/iphone-13-pro-camera-review-tanzania",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>No big deal — just a safari expedition to Tanzania. Lions, leopards, giraffes. Ultra wide angle 4K 60 video shot from an iPhone 13 Pro mounted to a helicopter. Your typical iPhone camera review.</p>\n\n<p>The review starts with a terrific movie — including some truly pro-looking Cinematic mode shots — by <a href=\"https://mckayfilms.com\">Taylor McKay</a>.</p>\n\n<p>I thought this was a pretty interesting observation from Mann:</p>\n\n<blockquote>\n  <p>Although the iPhone 13 Pro still only has three lenses, the\naddition of macro capability is like adding a new lens altogether,\nand for the serious photographer I think it’s perhaps the\nstrongest advancement in this year’s camera system. […]</p>\n\n<p>Photographer or not, you’ve seen the big and heavy backpacks\nphotographers carry with them on every shoot. Whether it’s local\nor international, we lug these bags full of lenses around because\neach one offers a new perspective on whatever story it is that\nwe’re telling.</p>\n\n<p>As a photographer passionate about the natural world, I carry a\nmacro lens with me no matter what project I’m working on, just\nbecause I never know what tiny detail of interest might present\nitself. Now with the macro capability of the iPhone 13 Pro, I feel\nlike I have my “in-a-pinch” macro shots covered and I can leave\nthe rarely-used macro lens at home.</p>\n</blockquote>\n\n<p>Everything you see in this video was shot with a $1,000 device meant to fit in your pocket.</p>\n\n<p>Some great iOS 15 tips from Mann, too, including using the new Focus feature to create a custom “Shoot Mode” with no notifications whenever he’s using the Camera app or Halide. Also, Mann’s custom Photographic Style settings.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://austinmann.com/trek/iphone-13-pro-camera-review-tanzania\">austinmann.com/trek/iphone-13-pro-camera-review-tanzania</a></strong></em></p>\n"
      },
      {
         "title" : "Software Update Adds Bluetooth Audio Support to the Nintendo Switch, Four Years After It Debuted",
         "date_published" : "2021-09-23T20:34:19Z",
         "date_modified" : "2021-09-23T20:37:45Z",
         "id" : "https://daringfireball.net/linked/2021/09/23/nintendo-switch-bluetooth-audio-finally",
         "url" : "https://daringfireball.net/linked/2021/09/23/nintendo-switch-bluetooth-audio-finally",
         "external_url" : "https://twitter.com/NintendoAmerica/status/1437930124490457088",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>A story like this is why you shouldn’t misuse <em>finally</em> in headlines. Four years!</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://twitter.com/NintendoAmerica/status/1437930124490457088\">twitter.com/NintendoAmerica/status/1437930124490457088</a></strong></em></p>\n"
      },
      {
         "title" : "How Apple Built the iPhone 13’s Cinematic Mode",
         "date_published" : "2021-09-23T20:18:32Z",
         "date_modified" : "2021-09-23T20:28:03Z",
         "id" : "https://daringfireball.net/linked/2021/09/23/panzarino-cinematic-mode",
         "url" : "https://daringfireball.net/linked/2021/09/23/panzarino-cinematic-mode",
         "external_url" : "https://techcrunch.com/2021/09/23/how-apple-built-the-iphone-13-pros-cinematic-mode/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Great interview by Matthew Panzarino with Apple vice president Kaiann Drance and human interface designer Johnnie Manzari from Apple’s Camera team:</p>\n\n<blockquote>\n  <p>That’s not even counting tracking shots, where a focus puller is\ncontinually adjusting focus as the camera moves and even the\nsubject moves in relation to the camera. It’s a highly skilled\noperation. To pull off a tracking shot, a focus puller must\npractice and train extensively for years. This, Manzari says, is\nwhere Apple sees an opportunity.</p>\n\n<p>“We feel like this is the kind of thing that Apple tackles the\nbest. To take something difficult and conventionally hard to\nlearn, and then turn it into something automatic and simple.”</p>\n\n<p>So the team started working through the technical problems in\nfinding focus, locking focus and racking focus. And these\nexplorations led them to gaze.</p>\n\n<p>“In cinema, the role of gaze and body movement to direct that\nstory is so fundamental. And as humans we naturally do this, if\nyou look at something, I look at it too.”</p>\n\n<p>So they knew they would need to build in gaze detection to help\nlead their focusing target around the frame, which in turn leads\nthe viewer through the story. Being on set, Manzari says, allowed\nApple to observe these highly skilled technicians and then build\nin that feel.</p>\n</blockquote>\n\n<p>Panzarino includes <a href=\"https://www.youtube.com/watch?v=3JcEG5Vjt-w\">this three-minute video consisting of nothing but Cinematic mode clips</a> from the trip to Disneyland he took with his family to test the new iPhones. There are some really neat shots in the video — I particularly like the one around the 1m:32s mark with his kids on the carousel. That change in focus is exactly what Cinematic mode was meant for.</p>\n\n<p>But the other thing that Panzarino’s video exemplifies is that you don’t have to <em>work</em> to use Cinematic mode. No help from someone else (let alone a crew), no extra lighting, no more difficult than just shooting a regular video mode clip. Something anyone could do — and might want to do — on a hectic day at a fun theme park. If you screw up the focus while shooting you can <em>easily</em> fix it — or just improve it — later.  </p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://techcrunch.com/2021/09/23/how-apple-built-the-iphone-13-pros-cinematic-mode/\">techcrunch.com/2021/09/23/how-apple-built-the-iphone-13…</a></strong></em></p>\n"
      },
      {
         "title" : "Apple’s Texas-Sized Problem",
         "date_published" : "2021-09-23T18:58:55Z",
         "date_modified" : "2021-09-23T21:19:25Z",
         "id" : "https://daringfireball.net/linked/2021/09/23/apple-texas-sized-problem",
         "url" : "https://daringfireball.net/linked/2021/09/23/apple-texas-sized-problem",
         "external_url" : "https://popular.info/p/apples-texas-problem",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Judd Legum, writing at Popular Information:</p>\n\n<blockquote>\n  <p>On Friday, CEO Tim Cook answered a question about Apple’s stance\non the Texas ban at an <a href=\"https://www.nytimes.com/2021/09/17/technology/apple-employee-unrest.html\">all-staff meeting</a>. Cook said that “the\ncompany was looking into whether it could aid the legal fight\nagainst the new law.”</p>\n\n<p>Apple has considerable leverage over the abortion debate in Texas\nand across the country — but it is not related to its ability to\npay for lawyers. Apple’s leverage rests in its status as a major\nemployer and driver of economic growth.</p>\n\n<p>If Apple believes that its employees should be able to “make their\nown decisions regarding their reproductive health,” it could\npublicly state that it will not expand its workforce in states\nthat limit abortion rights. That would have a major influence not\nonly in Texas but in <a href=\"https://popular.info/p/in-key-states-corporate-donations\">numerous states considering following Texas’\nlead</a>.</p>\n</blockquote>\n\n<p>Last week, <a href=\"https://techcrunch.com/2021/09/16/in-internal-memo-apple-says-it-is-monitoring-legal-challenges-to-texas-abortion-law/\">TechCrunch published the text of a company-wide memo</a> posted to an internal Apple message board regarding Texas’s near-outlawing of abortion. It began:</p>\n\n<blockquote>\n  <p>A message about women’s reproductive health care</p>\n\n<p>At Apple, we support our employees’ rights to make their own\ndecisions regarding their reproductive health.</p>\n</blockquote>\n\n<p>Legum is right — it’s untenable for Apple, or any other company, to “support our employees’ rights to make their own decisions regarding their reproductive health” <em>and</em> ask any woman to work for the company in a state with a law like Texas’s. An immediate hiring and construction freeze in Texas — explicitly tied to this outrageous law (which makes no exceptions for rape or incest) — is the only tenable action compatible with Apple’s stated values.</p>\n\n<p><a href=\"https://twitter.com/AoDespair/status/1439957619901411329\">David Simon, linking to Legum’s post</a>:</p>\n\n<blockquote>\n  <p>If an employer, this is beyond politics. I’m turning in scripts\nnext month on an HBO non-fiction miniseries based on events in\nTexas, but I can’t and won’t ask female cast/crew to forgo civil\nliberties to film there. What else looks like Dallas/Ft. Worth?</p>\n</blockquote>\n\n<p>That’s the answer. You move your business out of Texas. Any company that expands or initiates new operations in Texas implicitly supports Texas’s abortion ban.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://popular.info/p/apples-texas-problem\">popular.info/p/apples-texas-problem</a></strong></em></p>\n"
      },
      {
         "title" : "★ Apple Will Not Reinstate Epic’s Fortnite Developer Account, but Epic’s Other Developer Accounts Remain Active",
         "date_published" : "2021-09-23T01:29:18Z",
         "date_modified" : "2021-09-23T03:50:58Z",
         "id" : "https://daringfireball.net/2021/09/epic_apple_developer_accounts",
         "url" : "https://daringfireball.net/2021/09/epic_apple_developer_accounts",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p><a href=\"https://twitter.com/timsweeneyepic/status/1440711772483186690\">Tim Sweeney, today on Twitter</a>:</p>\n\n<blockquote>\n  <p>Late last night, Apple informed Epic that Fortnite will be\nblacklisted from the Apple ecosystem until the exhaustion of all\ncourt appeals, which could be as long as a 5-year process.</p>\n</blockquote>\n\n<p>Sweeney posted a letter from Apple’s attorneys to Epic’s. It reads:</p>\n\n<blockquote>\n  <p>September 21, 2021</p>\n\n<p>VIA ELECTRONIC MAIL</p>\n\n<p>Gary Bornstein <br />\nCravath, Swaine &amp; Moore LLP <br />\nWorldwide Plaza <br />\n825 Eighth Avenue <br />\nNew York, NY 10019-7475</p>\n\n<p>Re: Developer Program Account No. 8XJ6WJ8Z84</p>\n\n<p>Dear Gary,</p>\n\n<p>I am responding to your recent request that Apple reinstate Epic’s\ndeveloper program account, which was terminated for cause last\nyear. Epic committed an intentional breach of contract, and breach\nof trust, by concealing code from Apple and making related\nmisrepresentations and omissions. In its decision, the court\nrecognized that “Apple had contractual rights to act as It did. It\nmerely enforced those rights as [Epic’s] own internal documents\nshow Epic Games expected.” ECF No. 812 at 178-79. The court\nfurther found that “Apple’s termination of the [Developer Program\nLicense Agreement] and the related agreements between Epic Games\nand Apple was valid, lawful, and enforceable.” <em>Id.</em> at 179.\nFollowing that decision, Mr. Sweeney has publicly said that Epic\n“[w]ouldn’t trade [an alternative payment system] away to get\nFortnite back on iOS.” In light of this and other statements since\nthe court’s decision, coupled with Epic’s duplicitous conduct in\nthe past, Apple has exercised its discretion not to reinstate\nEpic’s developer program account at this time. Furthermore, Apple\nwill not consider any further requests for reinstatement until the\ndistrict court’s judgment becomes final and nonappealable.</p>\n\n<p>Sincerely,</p>\n\n<p>/s/ Mark A. Perry <br />\nMark A. Perry</p>\n</blockquote>\n\n<p>That’s lawyer-speak, I believe, for “go fuck yourselves”.<sup id=\"fnr1-2021-09-22-B\"><a href=\"#fn1-2021-09-22-B\">1</a></sup></p>\n\n<p><a href=\"https://twitter.com/TimSweeneyEpic/status/1440711467888615431\">Sweeney is crying foul</a>, arguing that this contradicts Apple’s repeated public statements that Fortnite would be welcomed back to the App Store <em>if they came into full compliance with App Store rules</em>. Here’s a version of Apple’s statement from two weeks ago, <a href=\"https://www.protocol.com/apple-blocks-epic-from-bringing-fortnite-back-to-the-app-store\">via Protocol</a>:</p>\n\n<blockquote>\n  <p>“As we’ve said all along, we would welcome Epic’s return to the\nApp Store if they agree to play by the same rules as everyone\nelse. Epic has admitted to breach of contract and as of now,\nthere’s no legitimate basis for the reinstatement of their\ndeveloper account.”</p>\n</blockquote>\n\n<p>Apple’s lawyers’ characterization of Sweeney’s statement about being unwilling to trade something away “to get Fortnite back on iOS” does seem like a bit of a hatchet-job, quote-editing-wise. <a href=\"https://twitter.com/TimSweeneyEpic/status/1440712310339694592\">Sweeney tweeted the following on September 11</a>, one day after the Epic-v.-Apple decision was delivered:</p>\n\n<blockquote>\n  <p>Thinking much more about whether we’re going to live in a world\nwhere two platform megacorps dictate software and world commerce\nto everyone or whether the digital world and the future metaverse\nwill be a free world. Wouldn’t trade that away to get Fortnite\nback on iOS.</p>\n</blockquote>\n\n<p>That doesn’t sound like the words of a man poised to comply with the App Store rules around in-app purchases. But, it doesn’t mean Epic <em>wasn’t</em> going to submit a Fortnite build that fully complies with the rules, either. Really does seem like Sweeney just thinking out loud in a tweet.</p>\n\n<p>Sweeney <em>also</em> <a href=\"https://twitter.com/TimSweeneyEpic/status/1440711578819567622\">tweeted an email</a> he sent to Phil Schiller on September 16. It reads:</p>\n\n<blockquote>\n  <p>From: Tim Sweeney <br />\nDate: Thu, Sep 16, 2021 at 5:01 PM <br />\nSubject: Fortnite and the App Store <br />\nTo: Phil Schiller  </p>\n\n<p>Hi Phil,</p>\n\n<p>I’m writing to provide clarity on where we stand.</p>\n\n<p>Epic has appealed the court’s decision in our suit over Apple’s\npolicies on In-App Purchase and competing stores. Though we can’t\nupdate the Fortnite version that users still have on their iOS\ndevices, we’ve disabled Epic payments server-side, and have paid\nApple $6,000,000 as ordered by the court.</p>\n\n<p>Epic has asked Apple to reactivate our Fortnite development\naccount. Epic promises that it will adhere to Apple’s guidelines\nwhenever and wherever we release products on Apple platforms.\nIf we get the account back, we’ll bring Fortnite back to Mac as\nsoon as possible, and we’ll reincorporate Fortnite for iOS in our\nUnreal Engine development and testing process, which will benefit\nall of our mutual developers.</p>\n\n<p>Whether Epic chooses to bring Fortnite back to iOS consumers\ndepends on whether and where Apple updates its guidelines to\nprovide for a level playing field between Apple In-App Purchase\nand other methods of payment.</p>\n\n<p>Epic will resubmit Fortnite to the App Store if you adhere to the\nplain language of the court order and allow apps to include\nbuttons and external links that direct customers to other\npurchasing mechanisms without onerous terms or impediments to a\ngood user experience. In that case, our remaining dispute will be\nabout competing stores, and I genuinely believe we could find\ncommon ground on the topic if Apple’s position were based solely\non user security and privacy rather than commercial interests.</p>\n\n<p>As a provider of developer tools, Epic continues to support Apple\nplatforms and our mutual developers wholeheartedly.</p>\n\n<p>If you have any questions or thoughts, I’m happy to talk.</p>\n\n<p>Tim Sweeney <br />\nEpic Games</p>\n</blockquote>\n\n<p>A few comments:</p>\n\n<blockquote>\n  <p>Epic promises that it will adhere to Apple’s guidelines whenever\nand wherever we release products on Apple platforms.</p>\n</blockquote>\n\n<p>Epic, of course, had previously promised the same thing, in a legally binding fashion, when they agreed to Apple’s developer account terms and conditions. But agreeing not to break Apple’s guidelines again seems in the spirit of what Apple had been asking for, regarding reinstating Fortnite.</p>\n\n<blockquote>\n  <p>Epic will resubmit Fortnite to the App Store if you adhere to the\nplain language of the court order and allow apps to include\nbuttons and external links that direct customers to other\npurchasing mechanisms without onerous terms or impediments to a\ngood user experience.</p>\n</blockquote>\n\n<p>Here’s where I think Sweeney garnered the legal “go fuck yourself”. Sweeney is arguing that Apple, which won the lawsuit, should interpret <a href=\"https://stratechery.com/2021/the-apple-v-epic-decision/\">the court’s anti-steering injunction</a> in a way that pleases Epic, which lost the lawsuit. That’s not how things work.</p>\n\n<blockquote>\n  <p>In that case, our remaining dispute will be about competing\nstores, and I genuinely believe we could find common ground on the\ntopic if Apple’s position were based solely on user security and\nprivacy rather than commercial interests.</p>\n</blockquote>\n\n<p>Tim Sweeney is high as a kite.</p>\n\n<hr />\n\n<p>So here’s the thing to keep in mind, and that I think Sweeney purposefully muddled in the way he announced this news: Epic is a conglomerate with multiple subsidiaries, and those subsidiaries have their own Apple Developer Program accounts. The only developer account Apple ever disabled in this dispute was the one held by Epic Games, Inc. — the Fortnite account. It was disabled on 28 August, 2020 and has been disabled ever since.</p>\n\n<p>Accounts that have never been disabled include the accounts for Rocket League (a game whose Mac support <a href=\"https://www.rocketleague.com/news/ending-support-for-mac-and-linux/\">Epic discontinued in January 2020</a>, exemplifying Epic’s “wholehearted” support for “Apple platforms”), and separately and importantly, Unreal Engine. It <em>is</em> true that Apple moved to block the Unreal Engine account back in August 2020, <a href=\"https://techcrunch.com/2020/08/24/apple-ordered-to-not-block-epic-games-unreal-engine-but-fortnite-to-stay-off-app-store/\">but Judge Yvonne Gonzalez Rogers ordered Apple not to pending a decision in the case</a>, while allowing the Fortnite account to be blocked. In her ruling this month, however, Gonzalez Rogers stated that Apple would now be within its rights to disable any and all of Epic’s Apple developer accounts for breaching the  license agreement. (See p. 179 of <a href=\"https://daringfireball.net/linked/2021/09/10/judgment-in-epic-v-apple\">the ruling</a>.)</p>\n\n<p>My understanding is that none of those accounts are affected by Apple’s decision not to reinstate the Fortnite developer account. Those accounts have been operational throughout this legal dispute, and I believe will continue to be — by Apple’s choice.</p>\n\n<div class=\"footnotes\">\n<hr />\n<ol>\n<li id=\"fn1-2021-09-22-B\">\n<p>Thank goodness lawyers seemingly always let you know in ALL CAPS when they send a letter via email, that they in fact SENT IT VIA ELECTRONIC MAIL.&nbsp;<a href=\"#fnr1-2021-09-22-B\"  class=\"footnoteBackLink\"  title=\"Jump back to footnote 1 in the text.\">&#x21A9;&#xFE0E;</a></p>\n</li>\n</ol>\n</div>\n\n\n\n    "
      },
      {
         "title" : "iPhone 13 and Apple Silicon",
         "date_published" : "2021-09-22T23:59:05Z",
         "date_modified" : "2021-09-23T00:16:10Z",
         "id" : "https://daringfireball.net/linked/2021/09/22/bajarin-iphone-13-apple-silicon",
         "url" : "https://daringfireball.net/linked/2021/09/22/bajarin-iphone-13-apple-silicon",
         "external_url" : "https://creativestrategies.com/iphone-13-and-apple-silicon/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Ben Bajarin, writing at Creative Strategies:</p>\n\n<blockquote>\n  <p>While I will admit there is a small percentage of Apple customers\nwho upgrade every year and a percentage more who upgrade every two\nyears because they are on upgrade plans, the vast majority of\nconsumers upgrade every 3-4 years. I thought it would be\ninteresting to look at some basic iPhone benchmarks through the\nyears and look at how much performance improvement happens every\nfour years.</p>\n</blockquote>\n\n<p>Incremental improvements every year turn into profound improvements over 3–4 years. It’s like the technology version of compound interest. It adds up.</p>\n\n<blockquote>\n  <p>As I benchmarked the A15 Bionic in different ways and pondered how\nApple spends its transistor budget with each A-series chip cycle,\nan interesting shift emerged for iPhone 13. Going back to how\nApple spends their transistor budget on features, not necessarily\nperformance, for the A15, Apple looks to have had the most GPU\ngains YoY since the A9. For the past five years, Apple has had an\naverage of 19% GPU gains YoY but for the A15 Bionic, <em>Apple has\nincreased GPU performance by 52%</em>.</p>\n\n<p>This intentional increase in GPU performance over CPU performance\nspeaks to the more graphically intense features Apple had in mind\nfor iPhone 13 that is demonstrated in things like macro\nphotography, macro video, and Cinematic Mode. Developers also now\nhave a dramatically increased GPU at their disposal to create new\napp experiences around and can leverage new augmented reality\ntechniques, visual computing and AI, and more.</p>\n</blockquote>\n\n<p>It’s almost enough to make one think that Apple is ready to release high-end professional Macs built around Apple GPUs.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://creativestrategies.com/iphone-13-and-apple-silicon/\">creativestrategies.com/iphone-13-and-apple-silicon/</a></strong></em></p>\n"
      },
      {
         "title" : "Music Video Shot With iPhone 13 Pro Cinematic Mode: Julia Wolf — ‘Falling in Love’",
         "date_published" : "2021-09-22T22:58:40Z",
         "date_modified" : "2021-09-22T22:58:40Z",
         "id" : "https://daringfireball.net/linked/2021/09/22/cinematic-mode-morrison-video",
         "url" : "https://daringfireball.net/linked/2021/09/22/cinematic-mode-morrison-video",
         "external_url" : "https://www.youtube.com/watch?v=Ae19-qqIMbQ",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Jonathan Morrison:</p>\n\n<blockquote>\n  <p>Went hands on with the iPhone 13 Pro and immediately wanted to\ntest out the camera and cinematic mode. It’s limited to 1080p\n30fps but I was surprised to see how sharp it was AND that it\nretained Dolby Vision.</p>\n</blockquote>\n\n<p>Interesting to see Cinematic mode in the hands of a talented videographer. Easily the best “in the wild” Cinematic mode video I’ve seen. (Explicit lyrics in the song.)</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.youtube.com/watch?v=Ae19-qqIMbQ\">youtube.com/watch?v=Ae19-qqIMbQ</a></strong></em></p>\n"
      },
      {
         "title" : "Wired’s 2011 Review of the iPhone 4S",
         "date_published" : "2021-09-22T22:07:39Z",
         "date_modified" : "2021-09-22T22:08:14Z",
         "id" : "https://daringfireball.net/linked/2021/09/22/wired-2011-iphone-4s-review",
         "url" : "https://daringfireball.net/linked/2021/09/22/wired-2011-iphone-4s-review",
         "external_url" : "https://www.wired.com/2011/10/iphone4s/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>From Wired’s review of the iPhone 4S:</p>\n\n<blockquote>\n  <p>Apple never specified what the “S” stands for in iPhone 4S, and it\nmay as well stand for Siri. Sure, the fifth-generation iPhone’s\nsuperb camera and speedy dual-core processor are classy additions.\nBut Siri is the reason people should buy this phone. […]</p>\n\n<p>The iPhone 4S looks exactly the same as its predecessor — but who\ncares? If it was shaped even slightly differently or came in a new\ncolor, people would still go nuts over the stuff that’s more\nimportant anyway: the insides. And both inside and out, this is a\nmagnificent smartphone.</p>\n\n<p>The late Steve Jobs once called the computer the equivalent of a\nbicycle for our minds. I think of the smartphone as the rocket\nship for our minds. With increasingly powerful sensors and\ntechnologies, and access to hundreds of thousands of apps enabling\nus to do just about anything, the iPhone keeps soaring to\nincredible heights and taking us to places with limitless\npotential. I guess that’s what you have to do to create a ding in\nthe universe.</p>\n</blockquote>\n\n<p>I don’t know what happened to the fellow who wrote this review 10 years ago, but The New York Times <a href=\"https://daringfireball.net/linked/2021/09/22/review-from-another-planet\">could sure use</a> a personal tech critic with this sort of enthusiasm and insight into the way that incremental improvements aggregate in just a few years in profound ways.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.wired.com/2011/10/iphone4s/\">wired.com/2011/10/iphone4s/</a></strong></em></p>\n"
      },
      {
         "title" : "‘The Most Important iPhone Ever’",
         "date_published" : "2021-09-22T21:35:10Z",
         "date_modified" : "2021-09-23T00:07:29Z",
         "id" : "https://daringfireball.net/linked/2021/09/22/dediu-most-important-iphone-ever",
         "url" : "https://daringfireball.net/linked/2021/09/22/dediu-most-important-iphone-ever",
         "external_url" : "http://www.asymco.com/2021/09/21/the-most-important-iphone-ever/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Horace Dediu, writing at Asymco:</p>\n\n<blockquote>\n  <p>There are more than 1 billion iPhone users. The total number of\nusers has been rising steadily. iPhone users make up about 26% of\nall smartphone users (3.8 billion is the current estimate). The\nshare of users in the US is about 60% (or soon will be.) The share\nin UK is close to 50%. All these share numbers are higher than\never. Over 14% of US and 10% of UK survey respondents have\nswitched to an iPhone in the past two years.</p>\n</blockquote>\n\n<p>I was not aware that churn was so strongly in the favor of iPhone over the last two years. Pretty good for a phone that <a href=\"https://daringfireball.net/linked/2012/01/24/blodget\">Henry Blodget declared “dead in the water”</a> in 2012. The downside to this trend, if it continues, is Apple might start running into being deemed an actual monopolist — by which I mean holding a monopoly share of <em>phones</em> period, not just a monopoly on iPhones. And with its sole OS competitor <a href=\"https://daringfireball.net/linked/2020/06/25/wong-ios-14-android\">increasingly showing signs</a> of <a href=\"https://daringfireball.net/linked/2020/07/20/state-of-google-pixel\">losing institutional interest</a> in Android, that trend might continue.</p>\n\n<p>Dediu on the iPhone 13 and Apple’s camera improvements over the last few years in general:</p>\n\n<blockquote>\n  <p>We did not ask for rack focus, post-production focus (!), night\nmode, macro photography and portrait bokeh. But once we have these\nfeatures we begin, ever so slowly, to use them and then we start\ndemanding them. Conversely it seems that what people mostly ask\nfor — that is what the critics ask for — are extrapolations of\nexisting features. The “faster horse” dilemma.</p>\n</blockquote>\n\n<p>On the surface, the physics of photography are stacked against Apple. Apple’s “cameras” are pancake-thin phones that people rightfully expect to comfortably carry in a jeans pocket. The technically-best photos and videos you can create today are shot using very large, very heavy cameras. But in a very meaningful way, this severe disadvantage works in Apple’s favor. It’s good to be the underdog. It keeps you hungry. And in photography, Apple is very much the underdog — not to any competing company but to the laws of physics. They’ve been making better smartphones than their competition since the day the first iPhone went on sale. That can make a company lazy, and lose focus. The worst thing that ever happened to the Mac was Microsoft Windows going to shit after Windows XP. </p>\n\n<p>But Apple will be chasing “real” cameras in image quality for at least another decade, maybe forever. Settling for nothing less than making the best cameras, period, despite the severe form factor constraints of a “phone”, is the sort of north star that keeps a company focused.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"http://www.asymco.com/2021/09/21/the-most-important-iphone-ever/\">asymco.com/2021/09/21/the-most-important-iphone-ever/</a></strong></em></p>\n"
      },
      {
         "title" : "★ The 2021 iPad Mini",
         "date_published" : "2021-09-22T18:58:16Z",
         "date_modified" : "2021-09-23T00:04:47Z",
         "id" : "https://daringfireball.net/2021/09/the_2021_ipad_mini",
         "url" : "https://daringfireball.net/2021/09/the_2021_ipad_mini",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>I don’t generally lead with benchmarks or pricing, but here’s a thought about the new iPad Mini, which comes equipped with a version of the same A15 chip as the new iPhone 13 and 13 Pro models: For $500, you can buy an iPad that’s more or less as fast, if not faster, at single-threaded CPU performance as an M1 Mac.</p>\n\n<p>That’s a tremendous value. The iPad Mini even has an A15 with an extra (fifth) GPU core, like the iPhone 13 Pro.</p>\n\n<p>Upgrading from 64 to 256 GB of storage costs $150; upgrading to add cellular support costs $150. So a maxed out iPad Mini — 256 GB of storage plus cellular support — costs $800. (There are only two storage options, 64 and 256 GB.) It’d be nice if — like all the new iPhone 13 models — the base storage were 128 GB instead of 64. But, still, the new iPad Mini is a terrific little tablet, and has performance that should keep it very useful for many years to come.</p>\n\n<p>It is, effectively, an iPad <em>Air</em> Mini. <a href=\"https://www.apple.com/ipad/compare/?modelList=ipad-air-4th-gen,ipad-mini-6th-gen,ipad-9th-gen\">Just like the iPad Air</a>, the new Mini sports a round-cornered display, no home button, and Touch ID on the power button. The new no-adjective entry-level iPad still has a square-cornered display, and Touch ID on a traditional home button on the front face. Also like the current iPad Air, the new iPad Mini uses a USB-C port instead of Lightning, and thus uses the superior magnetic second-generation Apple Pencil.</p>\n\n<p>Because the Mini is brand new and the current Air came out last October, the Mini was able to pull ahead in certain respects: A15 instead of A14, 5G support on cellular models, and a better front-facing camera (12 MP vs. 7 MP) — including support for <a href=\"https://support.apple.com/en-us/HT212315\">Center Stage</a>, Apple’s recent feature that dynamically adjusts the front-facing camera’s field of view depending on how many people are in the frame and where they are.  The rear cameras of the Air and Mini are similarly specced, and to my eyes shoot equivalent quality photos and video, but the new iPad Mini includes True Tone LED flash. The big win to me is the upgraded front-facing camera with Center Stage support. I’m not sure if you’ve heard, but video calls have become a big deal over the last two years.</p>\n\n<p>I think most iPad Mini fans would have been delighted if the new model were specced <em>exactly</em> like the current iPad Air, at these same prices. (The iPad Air costs $100 more than the equivalent Mini for the same amount of storage — $600 for 64 GB, $750 for 256 GB — but it only costs $130 to add cellular support to the Air. I suspect the difference in cellular model pricing is a 5G thing.) That the iPad Mini offers several technical advantages over last year’s iPad Air is pure gravy.</p>\n\n<p>I’ve been using the new iPad Mini for a week. As is my tradition for reviews of and first looks at new iPad models, I’m <a href=\"/misc/2021/09/ipad-mini-k2-keyboard-magic-trackpad.jpeg\">writing this piece on the iPad Mini itself</a>, using <a href=\"https://www.keychron.com/products/keychron-k2-wireless-mechanical-keyboard\">a bluetooth keyboard</a> and Magic Trackpad. It’s a nice small-footprint setup. The smaller text on the Mini’s smaller display is a little hard on my aging and somewhat problematic eyes while sitting at hardware keyboard distance, but my biggest annoyance is the lack of Face ID. I’m spoiled by my 2018 iPad Pro — while using a keyboard with an iPad, I expect to both wake it up <em>and</em> unlock it by just pressing the space bar or any other key. Having to reach over and touch the Touch ID button on the iPad is, simply, an inferior experience compared to Face ID. And it’s especially hard for me, right now, after a few years of expecting Face ID to just work with an iPad connected to a keyboard. I felt the same way writing <a href=\"https://daringfireball.net/2020/10/the_2020_ipad_air\">last year’s piece on the iPad Air</a>.</p>\n\n<p>If you don’t already have a Face ID habit using your iPad, however, this should be no big deal at all. Perhaps it’s even unfair for me to complain about, given that I do the vast majority of my writing on an M1 MacBook Pro — which also uses Touch ID, not Face ID. But maybe it <em>is</em> fair to complain about, because on a MacBook the Touch ID button is right on the keyboard — much more convenient to reach — and Macs support unlocking via the proximity of your Apple Watch. I think it’d be very cool if iPadOS supported unlocking via Apple Watch, much like MacOS does.</p>\n\n<p>All that said, if you’re the sort of person who’d like to do a lot of writing on an iPad Mini, you’ll be fine.</p>\n\n<p>One interesting change is that the hardware volume buttons have moved to the same side of the device as the power/Touch ID button. That means the volume buttons are on top when the iPad is in vertical orientation, and on the left side of the device when horizontal. The reason for this is obvious when you think about it, and consider the size of an Apple Pencil. Speaking in vertical (a.k.a. portrait) orientation terms, the Pencil, when attached, doesn’t leave any room for volume buttons on the right side of the device. But the volume buttons can’t go on the left side, because they’d get covered up when you connect a cover (like Apple’s own Smart Folio, which is very nice — the English lavender Smart Folio that Apple provided me with pairs nicely with the purple iPad Mini.) So, the volume buttons moved.</p>\n\n<p>One quibble: there are a few aspects of iPadOS that to me feel optimized only for larger iPads. The home screen Dock, for example, accepts up to 16 apps and folders. In vertical orientation, those icons are <em>really</em> tiny. Almost comically so. Yet in the same orientation, iPadOS will only display 5 apps in the Command-Tab switcher when you have a keyboard connected. I’m more annoyed by having just 5 apps in the Command-Tab switcher than by having super-small icons in my Dock, because I can adjust the number of apps in my Dock (by dragging a few lesser-used ones out) but I can’t adjust the maximum number of apps in the Command-Tab switcher. <a href=\"/misc/2021/09/ipad-mini-dock-versus-switcher.jpeg\">Here’s a screenshot</a>, but viewing it on another device won’t do justice to the feeling of just how small those Dock icons are, and just how comfortably a few more apps could fit in the switcher. It’s hard to put a finger on it,<sup id=\"fnr1-2021-09-22\"><a href=\"#fn1-2021-09-22\">1</a></sup> but there are just certain visual elements in iPadOS that feel inconsiderately shrunken on the iPad Mini, in a way that is <em>not</em> true for iOS on an iPhone Mini.</p>\n\n<p>A corresponding anti-quibble: After a fairly long stretch of not using an iPad Mini, I’m reminded how much nicer I find this size for typing with the on-screen keyboard compared to my 11-inch iPad Pro, because I can type with my thumbs, iPhone-style. I have never taken to typing on-screen on an iPad with my fingers, touch-typing-style, and at this point — over a decade into the iPad era — I doubt I ever will. As with the iPhone, I wouldn’t want to write anything long-form using just my thumbs on the on-screen keyboard, but it’s fine for dashing off text messages, tweets, and short emails. And, even better: <a href=\"https://twitter.com/gruber/status/1440816307381817346\">the iPad Mini still supports splitting the keyboard in two</a>, to make thumb-typing even easier. (It continues to baffle me that the iPad Pros do not support split keyboard mode.) If you like the idea of using an iPad as a sort of big-ass iPhone, the iPad Mini is obviously the iPad for you.</p>\n\n<div class=\"footnotes\">\n<hr />\n<ol>\n<li id=\"fn1-2021-09-22\">\n<p>No pun intended, I swear, vis-à-vis my complaint about tiny icons in the Dock.&nbsp;<a href=\"#fnr1-2021-09-22\"  class=\"footnoteBackLink\"  title=\"Jump back to footnote 1 in the text.\">&#x21A9;&#xFE0E;</a></p>\n</li>\n</ol>\n</div>\n\n\n\n    "
      },
      {
         "title" : "Who Needs to Shoot Photos in Low Light Anyway?",
         "date_published" : "2021-09-22T14:48:29Z",
         "date_modified" : "2021-09-22T22:18:29Z",
         "id" : "https://daringfireball.net/linked/2021/09/22/review-from-another-planet",
         "url" : "https://daringfireball.net/linked/2021/09/22/review-from-another-planet",
         "external_url" : "https://twitter.com/reckless/status/1440309785295933447",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Nilay Patel, on Brian X. Chen’s iPhone 13 review for <s>Pravda</s> The New York Times:</p>\n\n<blockquote>\n  <p>The NYT does not believe regular people stand to benefit from\nbetter iPhone photos in the dark. I live for this review from\nanother planet every year.</p>\n</blockquote>\n\n<p>I thought this was a really strange passage too. Quoting from <a href=\"https://www.nytimes.com/2021/09/21/technology/personaltech/apple-iphone13-review.html\">Chen’s review</a>:</p>\n\n<blockquote>\n  <p>So in summary, the iPhone 13 cameras are slightly better than\nthose of last year’s iPhones. Even compared with iPhones from\nthree years ago, the cameras are much better only if you care\nabout taking nice photos in the dark.</p>\n\n<p>Just how important is night photography? I posed the question to\nJim Wilson, a longtime staff photographer for The New York Times,\nas he was taking pictures of the new iPhones for this review. He\nsaid it would be a crucial feature for people like him, but not as\nimportant for casual shooters.</p>\n</blockquote>\n\n<p>I enjoy how Chen’s review opens with an egalitarian slam that Apple and Samsung’s annual phone updates are “a mirage of tech innovation” and instead are “a celebration of capitalism”, but when it comes to explaining why typical users shouldn’t care about low-light photography, he basically says “<em>because a professional staff photographer at The New York Times says they shouldn’t care</em>”.</p>\n\n<p><a href=\"https://twitter.com/benthompson/status/1440601049245491200\">Ben Thompson recalled</a> (as <a href=\"https://daringfireball.net/2019/09/you_could_always_just_use_flash\">I should have</a>, but did not) that this is something of a recurring theme. From <a href=\"https://www.nytimes.com/2019/09/17/technology/personaltech/iphone-11-review.html\">Chen’s review of the iPhones 11 and 11 Pro two years ago</a>:</p>\n\n<blockquote>\n  <p>Photos taken with the iPhone 11 and 11 Pro looked crisp and clear,\nand their colors were accurate. But after I finished these tests,\nI looked back at my archived photos taken with an iPhone X.</p>\n\n<p>Those pictures, especially the ones shot with portrait mode, still\nlooked impressive. Some of the low-light ones looked crummy in\ncomparison with the ones taken by the iPhone 11s, but I wouldn’t\nrecommend that you buy a new phone just to get better night\nphotos. You could always just use flash.</p>\n</blockquote>\n\n<p>“<em>You shouldn’t feel the need to buy a new iPhone every year</em>” is a fine sentiment, one that many, if not most, reviewers make each year. Arguing, repeatedly, that your readers should not be concerned at all about taking better photos in low light is bizarre. The single biggest change in consumer photography over the last 3–4 years is the exponential improvement in low light and night mode photography on new mobile phones.</p>\n\n<p>And again, <a href=\"https://daringfireball.net/linked/2021/09/21/chen-iphones-13\">as I mentioned yesterday</a>, Chen’s iPhone 13 review doesn’t even mention battery life, even though almost every other reviewer noted significant improvements across the lineup.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://twitter.com/reckless/status/1440309785295933447\">twitter.com/reckless/status/1440309785295933447</a></strong></em></p>\n"
      },
      {
         "title" : "Brian X. Chen on the iPhones 13: ‘The Most Incremental Upgrade Ever’",
         "date_published" : "2021-09-21T22:44:36Z",
         "date_modified" : "2021-09-21T22:44:36Z",
         "id" : "https://daringfireball.net/linked/2021/09/21/chen-iphones-13",
         "url" : "https://daringfireball.net/linked/2021/09/21/chen-iphones-13",
         "external_url" : "https://www.nytimes.com/2021/09/21/technology/personaltech/apple-iphone13-review.html",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Brian X. Chen’s review of the new iPhones for The New York Times is the least enthusiastic I’ve seen:</p>\n\n<blockquote>\n  <p>This is all to say the annual phone upgrade, which companies like\nApple and Samsung tout with enormous marketing events and ad\ncampaigns to gin up sales for the holiday shopping season, has\nbecome a mirage of tech innovation. In reality, the upgrades are\nnow a <a href=\"https://www.nytimes.com/2021/08/12/technology/new-smartphone-models.html\">celebration of\ncapitalism</a>\nin the form of ruthless incrementalism.</p>\n</blockquote>\n\n<p>Fair enough, but I found it curious that Chen’s review didn’t contain the word “battery”. The <a href=\"https://www.techmeme.com/210921/p18#a210921p18\">consensus is pretty strong</a> that the two standout features are better cameras and improved battery life.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.nytimes.com/2021/09/21/technology/personaltech/apple-iphone13-review.html\">nytimes.com/2021/09/21/technology/personaltech/apple…</a></strong></em></p>\n"
      },
      {
         "title" : "Joanna Stern: ‘From Mini to Pro Max, It’s All About the Battery and Cameras’",
         "date_published" : "2021-09-21T21:32:16Z",
         "date_modified" : "2021-09-21T21:32:16Z",
         "id" : "https://daringfireball.net/linked/2021/09/21/stern-iphone-13-cinematic-mode",
         "url" : "https://daringfireball.net/linked/2021/09/21/stern-iphone-13-cinematic-mode",
         "external_url" : "https://www.wsj.com/articles/iphone-13-pro-max-mini-review-11632223198",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Joanna Stern, reviewing the iPhone 13 lineup for the WSJ:</p>\n\n<blockquote>\n  <p>With videos, gosh, I was really excited about the new Cinematic\nmode. Aaaand gosh, was it a let down. The feature — which you\ncould call “Portrait mode for video” — adds artistic blur\naround the object in focus. The coolest thing is that you can\ntap to refocus while you shoot (and even do it afterward in the\nPhotos app).</p>\n\n<p>Except, as you can see in my video, the software struggles to know\nwhere objects begin and end. It’s a lot like the early days of\nPortrait Mode, but it’s worse because now the blur moves and\nwarps. I shot footage where the software lost parts of noses and\nfingers, and struggled with items such as a phone or camera. The\nApple spokeswoman said Cinematic mode is a “breakthrough\ninnovation that will keep getting better over time.”</p>\n</blockquote>\n\n<p>Stern went all-in on Cinematic mode for the video accompanying her review.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.wsj.com/articles/iphone-13-pro-max-mini-review-11632223198\">wsj.com/articles/iphone-13-pro-max-mini-review-11632223198</a></strong></em></p>\n"
      },
      {
         "title" : "Raymond Wong’s iPhone 13 Pro Review for Input",
         "date_published" : "2021-09-21T21:04:19Z",
         "date_modified" : "2021-09-22T14:17:43Z",
         "id" : "https://daringfireball.net/linked/2021/09/21/wong-iphone-13-pro",
         "url" : "https://daringfireball.net/linked/2021/09/21/wong-iphone-13-pro",
         "external_url" : "https://www.inputmag.com/reviews/iphone-13-pro-max-review-a-mighty-upgrade-thats-just-shy-of-perfect",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Raymond Wong shot a bunch of great camera comparisons for his Input review. He was annoyed by the same jarring automatic switch between the 1× to 0.5× lens when entering or leaving macro mode that I mentioned <a href=\"https://daringfireball.net/2021/09/the_iphones_13\">in my review</a>:</p>\n\n<blockquote>\n  <p>I welcome greater detail for close-ups and it’s clever that Apple\nis using the ultra-wide to augment the 1× wide and 3× telephoto at\nshort distances, but the transitioning of cameras is disorienting.\nApple makes no mention of this camera switching/augmenting on its\niPhone 13 Pro website. I get that it’s supposed to be one of those\n“it just works” features. At least that was Apple’s intention I’m\ntold, but it just doesn’t.</p>\n\n<p>Here’s a screen recording of the automatic camera switching in\naction. In this shot, I was trying to frame these delicious soup\ndumplings using the grid. Holding the iPhone 13 Pro still, you can\nsee the 1× wide switching to another slightly different FOV that’s\nusing the ultra-wide autofocusing. The viewfinder keeps jittering\nas it tries to choose between a regular wide or wide-macro shot. A\nregular person wouldn’t look at this and think to themselves, this\nis <em>normal</em>. They’d look at the jittering and think something is\nbroken with their iPhone camera. The framing should <em>never</em> change\nfrom what you compose and never automatically.</p>\n</blockquote>\n\n<p>Wong’s screen recording illustrates the issue perfectly.</p>\n\n<blockquote>\n  <p>When I first pressed Apple and made them aware of the jarring\ncamera switching, I was told it’s how the camera system works. On\nthe eve of this review, Apple changed course and said it’s going\nto release a software update to let users disable the camera\nswitching. According to Apple:</p>\n\n<blockquote>\n  <p>A new setting will be added in a software update this fall to turn\noff automatic camera switching when shooting at close distances\nfor macro photography and video.</p>\n</blockquote>\n</blockquote>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.inputmag.com/reviews/iphone-13-pro-max-review-a-mighty-upgrade-thats-just-shy-of-perfect\">inputmag.com/reviews/iphone-13-pro-max-review-a-mighty…</a></strong></em></p>\n"
      },
      {
         "title" : "Panzarino Takes the iPhone 13 Pro to Disneyland",
         "date_published" : "2021-09-21T20:54:31Z",
         "date_modified" : "2021-09-21T20:54:32Z",
         "id" : "https://daringfireball.net/linked/2021/09/21/panzarino-iphone-13-disneyland",
         "url" : "https://daringfireball.net/linked/2021/09/21/panzarino-iphone-13-disneyland",
         "external_url" : "https://techcrunch.com/2021/09/21/the-iphone-13-pro-goes-to-disneyland/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Matthew Panzarino, writing for TechCrunch, regarding Cinematic video mode:</p>\n\n<blockquote>\n  <p>I did some test shooting with my kids walking through crowds and\nriding on carousels that was genuinely, shockingly good. It really\ndoes provide a filmic, dreamy quality to the video that I was\npreviously only able to get with quick and continuous focus\nadjustments on an SLR shooting video with a manually focused lens.</p>\n\n<p>That, I think, is the major key to understanding Cinematic Mode.\nDespite the marketing, this mode is intended to unlock new\ncreative possibilities for the vast majority of iPhone users who\nhave no idea how to set focal distances, bend their knees to\nstabilize and crouch-walk-rack-focus their way to these kinds of\ntracking shots. It really does open up a big bucket that was just\ninaccessible before. And in many cases I think that those willing\nto experiment and deal with its near-term foibles will be\nrewarded with some great looking shots to add to their iPhone\nmemories widget.</p>\n</blockquote>\n\n<p>That sounds right to me.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://techcrunch.com/2021/09/21/the-iphone-13-pro-goes-to-disneyland/\">techcrunch.com/2021/09/21/the-iphone-13-pro-goes-to…</a></strong></em></p>\n"
      },
      {
         "title" : "Dieter Bohn on the iPhone 13 Pro",
         "date_published" : "2021-09-21T20:28:32Z",
         "date_modified" : "2021-09-21T20:28:49Z",
         "id" : "https://daringfireball.net/linked/2021/09/21/bohn-iphone-13-pro",
         "url" : "https://daringfireball.net/linked/2021/09/21/bohn-iphone-13-pro",
         "external_url" : "https://www.theverge.com/22684033/apple-iphone-13-pro-max-review",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Dieter Bohn, writing for The Verge:</p>\n\n<blockquote>\n  <p>Apple’s marketing for the camera system on the 13 Pro is that it’s\nthe “biggest advancement ever.” I don’t know that I would go that\nfar, but I also can’t remember the last time I’ve said “whoa, look\nat this photo” as many times as I have during this review. […]</p>\n\n<p>Where the Pro 13 camera system shines is in low light. The main\nwide-angle sensor has seen a massive upgrade this year. Unlike\nAndroid phones that are chasing big megapixel counts and then\n“pixel binning” to achieve low light performance, Apple is\nsticking with 12 megapixels, the same resolution it’s used since\n2015’s iPhone 6S. The sensor itself is much bigger now and\nfeatures 1.9 µm pixels, which are about as big as anything we’ve\nseen on a smartphone. And on top of all that, the lens now has an\nƒ/1.5 aperture.</p>\n\n<p>All of that adds up to a camera that can very quickly take in a\nmassive amount of light relative to other phones. Combined with\nsome tuning and improvements to Apple’s computational photography,\nthe low light performance on the 13 Pro is simply second to none.</p>\n</blockquote>\n\n<p>I came away super impressed with the low light performance of the 13 Pro, too.</p>\n\n<p>Bohn makes an important point in <a href=\"https://www.theverge.com/22684421/apple-iphone-13-mini-review\">his corresponding review of the 13 and 13 Mini</a> too: because the camera bumps are all new sizes, cases for the iPhone 13 won’t fit the 13 Pro, nor vice-versa.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.theverge.com/22684033/apple-iphone-13-pro-max-review\">theverge.com/22684033/apple-iphone-13-pro-max-review</a></strong></em></p>\n"
      },
      {
         "title" : "More, Smaller Apps",
         "date_published" : "2021-09-21T19:06:46Z",
         "date_modified" : "2021-09-21T19:06:47Z",
         "id" : "https://daringfireball.net/linked/2021/09/21/more-smaller-apps",
         "url" : "https://daringfireball.net/linked/2021/09/21/more-smaller-apps",
         "external_url" : "https://www.apple.com/newsroom/2021/08/apple-acquires-classical-music-streaming-service-primephonic/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Apple Newsroom, back on August 30:</p>\n\n<blockquote>\n  <p>Primephonic is no longer available for new subscribers and will be\ntaken offline beginning September 7. Apple Music plans to launch a\ndedicated classical music app next year combining Primephonic’s\nclassical user interface that fans have grown to love with more\nadded features. In the meantime, current Primephonic subscribers\nwill receive six months of Apple Music for free, providing access\nto hundreds of thousands of classical albums, all in Lossless and\nhigh-resolution audio, as well as hundreds of classical albums in\nApple Music’s Spatial Audio, with new albums added regularly.</p>\n</blockquote>\n\n<p>I’ve had this flagged for a few weeks. What I find interesting is Apple is going to use this acquisition to launch a dedicated classical music app, not to expand the Music app. iTunes, infamously, expanded greatly over the years, and everyone seems to agree that the user experience suffered for it. I wonder if that’s in the back of Apple’s mind here.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.apple.com/newsroom/2021/08/apple-acquires-classical-music-streaming-service-primephonic/\">apple.com/newsroom/2021/08/apple-acquires-classical-music…</a></strong></em></p>\n"
      },
      {
         "title" : "★ The iPhones 13",
         "date_published" : "2021-09-21T17:13:47Z",
         "date_modified" : "2021-09-24T14:16:45Z",
         "id" : "https://daringfireball.net/2021/09/the_iphones_13",
         "url" : "https://daringfireball.net/2021/09/the_iphones_13",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>I wish I had something more clever to say about the new iPhone 13 lineup. But the practical reality is simple and obvious. The two ways that Apple could best improve the day-to-day utility of using an iPhone are improving the camera system and improving battery life. And those are exactly where Apple focused its attention for this year’s new iPhones.</p>\n\n<p>In theory, another practical improvement would be to make phones that are thinner and lighter. But designing phones that are thinner and lighter would be in direct conflict with improving the cameras and battery life. You can’t have your cake and eat it too.</p>\n\n<p>All four new iPhones — the 13 Mini, the regular 13, the 13 Pro, and the 13 Pro Max — are the exact same height and width as the corresponding models from last year’s iPhone 12 lineup. But all four of the new iPhones are slightly thicker and heavier. The increase in thickness is very slight — from 7.4 mm to 7.65 mm. The increase in weight varies from around 5 to 7 percent. Not a lot, but you can feel it.</p>\n\n<p>The model with the biggest physical change year-over-year is the 6.1-inch 13 Pro. (Apple provided me with all four for testing, but I’ve spent most of my time over the last six days using the 13 Pro.) Last year, <a href=\"https://daringfireball.net/2020/11/the_iphone_12_mini_and_iphone_12_pro_max\">the 12 Pro Max had a much bigger camera module</a> on the back — bigger lenses that protrude more, and a bigger “platform” (“plateau”?) in which the lenses sit. This year, the 13 Pro and 13 Pro Max share the same camera module. You can both see and feel the difference on the 13 Pro compared to last year’s 12 Pro, or to any other previous iPhone in the “regular” size class.</p>\n\n<p>It is comical to look back at the minor controversy surrounding the iPhone 6 back in 2014. That was the first year the iPhone camera had a “bump”, which at the time seemed weird and obtrusive, even if the reason for the bump was obvious: improved optics. The controversy was that <a href=\"https://www.theverge.com/2014/9/16/6209759/apple-has-an-embarassing-bulge\">Apple’s promotional photography for the iPhone 6 seemed to go out of its way to hide that camera bump</a> — in a bunch of Apple’s profile shots, the back of the iPhone 6 looked perfectly flat. Apple deliberately chose angles and perspectives that did not show the camera bump, and headlines described the camera — that tiny little iPhone 6 camera — as an “embarrassing bulge”.</p>\n\n<p>Fast forward to today, and Apple is using photographs for the iPhone 13 Pro and Pro Max, that, if anything, <em>emphasize</em> the camera system’s size and prominence. Here’s a screenshot from <a href=\"https://www.apple.com/iphone-13-pro/\">Apple’s iPhone 13 Pro product page</a>:</p>\n\n<p><a href=\"/misc/2021/09/iphone-13-pro-camera-bump.jpeg\" class=\"noborder\">\n<img\n    src = \"/misc/2021/09/iphone-13-pro-camera-bump.jpeg\"\n    alt = \"A promotional photo of a silver iPhone 13 Pro emphasizing the prominence of its camera lenses.\"\n    width = 450\n/></a></p>\n\n<p>Nobody can claim Apple is hiding this “bump”. As with the 12 Pro Max last year, the camera systems on the 13 Pro and 13 Pro Max protrude so far that Apple’s cases for the devices have a prominent protective plastic lip around the camera cutout, such that even in a case, the iPhone wobbles when lying on a flat surface. (The cases for the iPhone 13 and 13 Mini have lips around the camera now, too, but they’re much smaller.)</p>\n\n<p>I’ve been arguing for years that iPhones are evolving such that they’re better thought of as cameras than “phones”. Now, there’s no need to argue about it. That’s especially true for the Pro models. What’s “pro” about the iPhone 13 Pro and Pro Max? The cameras. The “pro” prefix is right there in the name of camera features exclusive to the Pro devices: <a href=\"https://support.apple.com/en-us/HT211965\">ProRAW</a> and <a href=\"https://support.apple.com/en-us/HT202410\">ProRes</a>. I think it’s fair to say that the iPhone 13 and 13 Mini are phones with very good cameras; the 13 Pro and Pro Max are excellent cameras with phones.</p>\n\n<p>Computational photography is upending the entire camera world. It’s hard to beat the physics of good glass and large sensors, but math is doing pretty good — and gaining fast.</p>\n\n<h2>Performance, Efficiency, and ProMotion</h2>\n\n<p>During Apple’s keynote last week, the company didn’t mention year-over-year performance numbers for the A15 chip. This led to <a href=\"https://sixcolors.com/link/2021/09/a15-fast-and-slow/\">some speculation</a> that maybe the A15 isn’t much faster than the A14. But when benchmarks started leaking last week after phones got into reviewers’ hands, they showed performance improvements roughly in line with the improvements from the last few years: about 10 percent faster in single-threaded benchmarks, and about 20 percent faster in multi-threaded. That jibes with the numbers I saw using <a href=\"https://www.geekbench.com/\">GeekBench 5</a> and the web-based <a href=\"https://browserbench.org/Speedometer2.0/\">Speedometer benchmark</a>.</p>\n\n<p>Apple doesn’t like to explain itself, but I think they decided against emphasizing traditional benchmark-type figures (“<em>20 percent faster CPU performance, 40 percent faster machine learning</em>”, etc.) not because the A15 fares poorly in such comparisons, but because numbers like that don’t really tell the story of what the A15 is <em>about</em>. The more impressive year-over-year improvements are in battery life, and I think that’s largely about the efficiency of the A15. It is faster than the A14, by reasonable margins, but what’s more impressive is how much longer battery life is, with only a modest increase in device thickness.</p>\n\n<p>On the <a href=\"https://www.apple.com/iphone/compare/\">iPhone model comparison page</a>, Apple cites separate battery figures for “Video playback” and “Video playback (streamed)”. That’s something almost everyone does with their phones — stream video. A practical, real-world measure of battery life. Here are the year-over-year streaming video improvements for each of the four iPhones 12 and 13:</p>\n\n<ul>\n<li>iPhone 13 Mini: 13 hours, up from 10 hours last year on the 12 Mini.</li>\n<li>iPhone 13: 15 hours, up from 11 hours last year on the regular 12.</li>\n<li>iPhone 13 Pro: 20 hours, up from 11 hours last year on the 12 Pro.</li>\n<li>iPhone 13 Pro Max: 25 hours, up from 12 hours last year on the 12 Pro Max.</li>\n</ul>\n\n<p>Those are very big improvements for the non-pro iPhone 13 and 13 Mini. But the numbers for the 13 Pro and Pro Max are bananas. The Pro Max more than doubled its battery life for streaming video playback in a year. (!) All four iPhone 13 models are seeing benefits here from the A15 chip. But the Pro models are benefiting from a surprising direction: ProMotion. That’s Apple’s name for adaptive screen refresh rates. With the iPhone 13 Pro and Pro Max, the screen refresh rate ranges from as low as 10 Hz to as high as 120 Hz, and the system just manages it automatically based on what’s on screen. It’s the high refresh rates that garner attention — it’s a feature that makes scrolling look noticeably smoother. It just looks nicer.<sup id=\"fnr1-2021-09-21\"><a href=\"#fn1-2021-09-21\">1</a></sup> But, of course, updating the display at twice the refresh rate — 120 Hz instead of 60 — obviously consumes more power. </p>\n\n<p>This led to some speculation that the iPhone 13 Pro might get <em>worse</em> battery life than the regular iPhone 13, because ProMotion is exclusive to the 13 Pro and Pro Max. That speculation was based on the fact that high-end Android phones with high refresh rates — 90 or 120 Hz — <a href=\"https://www.anandtech.com/show/15765/120hz-on-the-oneplus-8-pro-qhd-resolution-but-still-power-hungry\">take noticeable hits to battery life</a>. What makes ProMotion different is that it’s adaptive. The showy-offy aspect of ProMotion is the high refresh rates, but the undeniable practical benefits are the adaptive <em>lower</em> refresh rates. That’s why the streaming video playback numbers for the 13 Pro and 13 Pro Max effectively doubled year-over-year: stream a video at 30 frames per second, and ProMotion will adapt the display refresh rate to 30 Hz. The adaptive nature of ProMotion means that not only does it not hurt battery life, like the less sophisticated high refresh rate features on Android phones, but it actually helps <em>extend</em> battery life for common tasks like watching video or reading text. Yes, the iPhone is late to the high refresh rate game, but as is often the case with Apple, it was worth waiting for.</p>\n\n<h2>Miscellaneous</h2>\n\n<ul>\n<li><p><span id = 'cinematic_mode'>Cinematic video mode</span> is a lot of fun. It’s a gimmick, yes, but I don’t mean that pejoratively. Gimmicks can be fun. Fun is good. I think people are going to use this feature to make videos that really will look more cinematic. It’s also nice that it’s not a feature exclusive to the Pro models. But like Portrait mode for stills, edge detection around subjects’ hair and eyeglasses can be hit or miss in Cinematic mode. Also, I find it a bit curious that Cinematic mode only shoots in one format: 1080p at 30 FPS. The 1080p limitation I understand — the ML-driven automatic subject detection and dynamically-created “bokeh” depth of field effect are clearly computationally expensive. But why not offer 24 FPS too? For reasons that have never been clear to me, Apple’s Camera app has only ever offered 24 FPS at 4K resolution, not at 1080p or 720p. The camera is certainly capable of it — plenty of third-party camera apps let you shoot 24 FPS video at 1080p and 720p, in addition to 4K. But only the system’s Camera app can shoot in Cinematic mode, a mode whose very name suggests “film style”, which is <a href=\"/misc/2021/09/24fps-film-style.jpeg\">exactly the term Apple itself uses in the Settings app to describe 4K 24 FPS</a>.</p></li>\n<li><p>Macro photography on the iPhone 13 Pro models is also a lot of fun. It’s almost like gaining a super power — the ability to see small objects and details far more clearly than with the naked eye. The way that macro mode kicks in automatically, though, can be a little jarring. How it works is, with a 1× field of view in the regular still photo mode, when you bring the camera very close to a subject or surface, the Camera app switches to the 0.5× ultra wide camera. But it’s not an ultra-wide field of view. You get a roughly 1× field of view but a very close focal distance. The jarring part is when the viewfinder switches between cameras — it’s like a jump cut. It’s understandable, and doesn’t dampen the utility or fun of the feature, but it’s a little weird every time you see it happen. It makes it feel not quite as automatic or modeless as Apple intends it to feel. Also, the built-in Magnifier app (Settings → Accessibility → Accessibility Shortcut) doesn’t seem to use the camera’s macro capability. For reading really tiny text — like, say, some of the <a href=\"https://www.mentalfloss.com/article/68109/15-microprints-hiding-united-states-currency\">hidden fine print on U.S. currency</a> — it’s far easier and more effective to use the Camera app than the Magnifier app.</p></li>\n<li><p>I bought a regular iPhone 12 last year for my personal use, but I’ve already ordered a 13 Pro this year. (Graphite, of course, because I’m boring that way.) The camera is just too good. Maybe the new 3× telephoto lens just feels like a lot of zoom to me, personally, because I’ve spent the last year mostly using an iPhone 12 that doesn’t have a telephoto lens of any sort, but it really feels like a lot of extra zoom compared even to a 2× iPhone camera from previous years.</p></li>\n<li><p>Polished stainless steel still feels like an odd material for a phone with flat sides. Somehow, to me, polished steel worked better for the round-sided iPhones (X, XS, 11). With the flat-sided iPhones 12 Pro and now 13 Pro, it’s a fingerprint magnet when used without a case. The aluminum iPhones 13 have better hand-feel to my taste, including the buttons.</p></li>\n<li><p>Colors: my review units are gold (13 Pro), sierra blue (13 Pro Max), midnight (13 Mini), and blue (regular 13). The gold once again is a very C-3PO gold. Sierra blue is very nice, and quite distinctive from any previous iPhone — I can see why Apple is using it a lot in their advertising. It plays as silver-y at times, but very clearly blue at others. Midnight plays as black or very dark gray, until you put it next to something truly black — it’s then apparent that midnight has a small touch of blue. It makes last year’s black iPhone 12 models look a little drab side-by-side. The non-pro iPhone 13 in just plain blue is nice. It’s a rich, vibrant blue. But <a href=\"https://daringfireball.net/2020/10/the_iphone_12_and_iphone_12_pro#fn7-2020-10-20\">once again</a>, the <a href=\"/misc/2021/09/no-blue-screws.jpeg\">screws on the bottom edge are not color matched</a>. The midnight iPhone 13 Mini has nearly-matching black screws, but the blue iPhone 13 has silver screws. I don’t know why that bugs me.</p></li>\n<li><p>Battery life was outstanding. As usual, I’ve been using the phone extensively, including power-hungry features like Cinematic mode, and I ended each day with plenty of charge left in the tank.</p></li>\n</ul>\n\n<div class=\"footnotes\">\n<hr />\n<ol>\n<li id=\"fn1-2021-09-21\">\n<p>It occurred to me while swiping to scroll a long web page as fast as I could that we’re <a href=\"https://daringfireball.net/2007/06/iphone_first_impressions\">a long way removed from the checkerboard placeholder background</a> that Mobile Safari would render while scrolling in iPhone OS version 1.&nbsp;<a href=\"#fnr1-2021-09-21\"  class=\"footnoteBackLink\"  title=\"Jump back to footnote 1 in the text.\">&#x21A9;&#xFE0E;</a></p>\n</li>\n</ol>\n</div>\n\n\n\n    "
      },
      {
         "title" : "[Sponsor] Retool",
         "date_published" : "2021-09-20T19:24:24-05:00",
         "date_modified" : "2021-09-20T19:24:25-05:00",
         "id" : "https://daringfireball.net/feeds/sponsors/2021/09/retool_1",
         "url" : "https://daringfireball.net/feeds/sponsors/2021/09/retool_1",
         "external_url" : "https://retool.com/?utm_source=sponsor&utm_medium=newsletter&utm_campaign=daringfireball",
         "authors" : [
            {
               "name" : "Daring Fireball Department of Commerce"
            }
         ],
         "content_html" : "\n<p>Programming has gotten surprisingly hard. Building a simple form to POST data back to your API means wrangling with redux and thunks. Oh, and debouncing that submit button. Everything but solving the business problem.</p>\n\n<p>Retool is a new approach: we’ve unified the ease of visual programming with the power and flexibility of real code. Drag and drop a form together, and have it POST back to your API in minutes. Deploy instantly with access controls and audit logs.</p>\n\n<p>Allbirds uses Retool to measure billboard efficacy. Amazon uses Retool to handle GDPR requests. You, too, can use it to build business-critical applications fast.</p>\n\n<p><a href=\"https://retool.com/?utm_source=sponsor&amp;utm_medium=newsletter&amp;utm_campaign=daringfireball\">Start building for free today</a>.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://retool.com/?utm_source=sponsor&utm_medium=newsletter&utm_campaign=daringfireball\">retool.com/?utm_source=sponsor&utm_medium=newsletter&utm…</a></strong></em></p>\n"
      },
      {
         "title" : "Listen Notes",
         "date_published" : "2021-09-18T18:26:43Z",
         "date_modified" : "2021-09-18T18:26:43Z",
         "id" : "https://daringfireball.net/linked/2021/09/18/listen-notes",
         "url" : "https://daringfireball.net/linked/2021/09/18/listen-notes",
         "external_url" : "https://www.listennotes.com/blog/why-podcasts-are-my-new-wikipedia-the-perfect-41/?s=df",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>My thanks to Wenbin Fang for sponsoring this week at DF to promote Listen Notes, a podcast search engine. He sponsored DF to share his story of how listening to podcasts has largely replaced Wikipedia as an informal learning resource for him, personally. </p>\n\n<p>Fang has used Listen Notes to help himself listen to about 5,000 podcast episodes in the past 4 years. (!) In his blog post, he explains his own idiosyncratic methods for podcast discovery and consumption.</p>\n\n<p>If you want to jumpstart your own podcast project, <a href=\"https://listennotes.com/api\">try the Listen Notes podcast API</a>, or if you want to find all podcast interviews of a person, just search for their name on <a href=\"https://www.listennotes.com/?s=df\">listennotes.com</a>. Just a website, really well done.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.listennotes.com/blog/why-podcasts-are-my-new-wikipedia-the-perfect-41/?s=df\">listennotes.com/blog/why-podcasts-are-my-new-wikipedia-the…</a></strong></em></p>\n"
      },
      {
         "title" : "The Talk Show: ‘It Was More Arial Than Helvetica’",
         "date_published" : "2021-09-18T18:17:28Z",
         "date_modified" : "2021-09-18T18:17:29Z",
         "id" : "https://daringfireball.net/linked/2021/09/18/the-talk-show-322",
         "url" : "https://daringfireball.net/linked/2021/09/18/the-talk-show-322",
         "external_url" : "https://daringfireball.net/thetalkshow/2021/09/18/ep-322",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Rene Ritchie returns to the show for a recap of this week’s “California Streaming” Apple Event: the iPhones 13, Apple Watch Series 7, and new iPads. Also, last week’s decision in the Apple v. Epic lawsuit.</p>\n\n<p>Brought to you by these fine sponsors:</p>\n\n<ul>\n<li><a href=\"https://squarespace.com/talkshow\">Squarespace</a>: Make your next move. Use code <strong>talkshow</strong> for 10% off your first order.</li>\n<li><a href=\"https://hellofresh.com/talkshow14\">Hello Fresh</a>: America’s #1 meal kit.</li>\n<li><a href=\"https://awaytravel.com/talkshow\">Away</a>: Designed to last for life.</li>\n</ul>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://daringfireball.net/thetalkshow/2021/09/18/ep-322\">daringfireball.net/thetalkshow/2021/09/18/ep-322</a></strong></em></p>\n"
      },
      {
         "title" : "★ Various Single-Paragraph Thoughts and Observations Regarding Yesterday’s ‘California Streaming’ Apple Event for the iPhones 13, Apple Watch Series 7, and New iPads",
         "date_published" : "2021-09-15T23:40:00Z",
         "date_modified" : "2021-09-16T09:41:00Z",
         "id" : "https://daringfireball.net/2021/09/california_streaming_thoughts_and_observations",
         "url" : "https://daringfireball.net/2021/09/california_streaming_thoughts_and_observations",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<h2>The Event</h2>\n\n<p>Staging-wise, I’m not sure I get Apple’s “let’s make this all about California” strategy. The footage from various scenic locations across the state was beautiful, but I don’t get why it mattered for this particular event. Apple’s always been in California, they’ve always been proud of being from California. My best guess is that it’s as simple as needing a theme of some sort, and “California scenic beauty” was as good as any, for yet another COVID era event that couldn’t be held inside with an audience. Joz presented outside at Apple Park, and Cook was on stage in the Steve Jobs theater, but I get the feeling they wanted to break away from Apple Park as the set dressing for the whole show, too.</p>\n\n<p>To that point, I thought Kaiann Drance’s segment introducing the iPhone 13 and 13 Mini was the most stunning. Standing on stage, alone, at <a href=\"https://www.sandiegosymphony.org/\">the San Diego Symphony’s outdoor theater</a>, in front of <a href=\"/misc/2021/09/drance-san-diego.jpeg\">all those empty seats</a>. It was both beautiful and an instant reminder of what we’re all missing.</p>\n\n<h2>The iPhones 13</h2>\n\n<p>Last year, the iPhone 12 and 12 Pro — the two “regular” sized new iPhones — shared the exact same protective cases. This year, there are different cases for the iPhone 13 and 13 Pro. I <em>think</em> that’s because the three-lens camera module on the back of the iPhone 13 Pro is bigger than the two-lens module on the iPhone 13. The width, height, and depth of the 13 Pro and regular 13 <a href=\"https://www.apple.com/iphone/compare/\">are identical</a>.</p>\n\n<p>Last year, the 12 Pro Max had a better camera system than the 12 Pro. Only the 12 Pro Max had the sensor shift optical image stabilization, and only the 12 Pro Max had a 2.5× (as opposed to 2×) telephoto lens. This year, both Pro models have identical camera systems. (And, like last year, the regular iPhone 13 and 13 Mini share the same camera system as each other.)</p>\n\n<p>The iPhone 13 Pro camera modules are entirely different from the non-Pro 13 and 13 Mini, though. Not just the existence of the new 3× telephoto, but the 1× (wide) and 0.5× (ultra wide) cameras are better on the Pro models. The 1× Pro camera has a maximum aperture of ƒ/1.5; the 1× non-Pro camera is ƒ/1.6. (Lower values for aperture let in more light; photographer lingo is that they’re “faster”.) The 0.5× Pro camera has a fast ƒ/1.8 aperture; the 0.5× non-Pro camera is ƒ/2.4.</p>\n\n<p>Macro photography is a Pro-only feature, I believe because the 13 Pro 0.5× ultra wide camera has autofocus, and the non-Pro 0.5× camera is fixed-focus.</p>\n\n<p>The front-facing camera on all iPhone 13 models appears to be the same, but only the Pro models can shoot in the ProRes format. (Not sure why anyone would want to shoot ProRes with the front-facing camera, though. But I guess why not enable it?)</p>\n\n<p>The AI-driven automatic focus changes in Cinematic Mode video seem too good to be true. Very futuristic feature, if it works as promised.</p>\n\n<p>I really missed having a hands-on experience with the new devices, if only to consider their colors. “Starlight” appears to be silver with a slight hint of gold. I’m tempted to say champagne, but maybe that implies too much gold. “Midnight” isn’t quite neutral dark gray or near-black — it has a hint of blue or indigo. (Blue is seemingly the color of the year. Anecdotally, it seems like a lot of people I know are planning to get the Pro models in Sierra Blue.)</p>\n\n<h2>Apple Watch Series 7</h2>\n\n<p>A bigger screen, with a brighter always-on display mode, and faster charging are OK year-over-year improvements. But clearly Series 7 is a minor, not major, refresh. That’s fine, and inevitable for a maturing product. You’re not supposed to buy a new $500 Apple Watch every year, and while I know a lot of people who buy a new iPhone each year (including yours truly), I don’t know anyone, even devout fitness enthusiasts, who buys a new Apple Watch annually. Even every other year feels pretty frequent. A Series 5 or Series 4, purchased new, should still be a really great Apple Watch. [<strong>Update:</strong> I should have known my audience better. A bunch of you buy a new Apple Watch every year. I think we can all admit it’s atypical, though — and that developers who buy a new one every year for testing are an edge case.]</p>\n\n<p><a href=\"https://twitter.com/SnazzyQ/status/1437902520731402242\">Quinn “Snazzy Labs” Nelson flagged Apple for an unfair comparison</a>, regarding just how much more text the larger Series 7 displays can show at a time. The font was the same size, but the line spacing was quite a bit tighter in the Series 7 screenshot. I would also argue that Apple chose text that line-wrapped <a href=\"http://www.eprg.org/G53DOC/pdfs/knuth-plass-breaking.pdf\">inefficiently</a> on the Series 6 display, but the difference in line heights is clearly unfair. Apple doesn’t usually play games like that in comparisons. Yellow card issued.</p>\n\n<p>The entry model $199 Apple Watch remains the now-kinda-long-in-the-tooth Series 3. I was really hoping for the Series 4 to take that spot in the lineup. I know developers of WatchOS apps were too. The Series 3 has an outdated screen size that developers are going to have to support for years to come.</p>\n\n<h2>New iPad Mini and 9th-Generation Just-Plain iPad</h2>\n\n<p>The iPad Mini has always been on a unique upgrade cycle. It goes years between refreshes, but when Apple does update it, they tend to bring it up to current specs. The new iPad Mini has the same A15 SoC as the iPhones 13 — in fact, it has the 5-core GPU like the iPhone 13 Pro models, not the 4-core GPU like the iPhone 13 and 13 Mini. The previous iPad Mini had the A12.</p>\n\n<p>The iPad Mini is really more like an iPad <em>Air</em> Mini. The new regular “iPad” still has a home button and sharp-cornered display. The Mini has the modern round-cornered display, no home button, and a Touch ID sensor on the power button — just like the current iPad Air. Also like the iPad Air, the new Mini has a USB-C port instead of Lightning. The volume buttons for the Mini are on the top of the device — a first for iPad. I’m guessing that decision was mainly about supporting the magnetic Pencil 2 along the long side of the device where the volume buttons traditionally go for iPads.</p>\n\n<h2>TV+ and Fitness+</h2>\n\n<p>One thought that occurred to me is that it’s good to see Apple pushing forward on their own original service products. Even putting aside the legal and legislative attention regarding the App Store — big things to put aside, at the moment — I just don’t think it’s healthy for Apple to depend on rent-seeking to grow Services revenue. Getting 30 percent of the revenue from subscriptions to other company’s services is a fine business, financially, but it’s like junk food for any company’s culture. Apple is a great company because they make great original things that people want to pay for. TV+ and Fitness+ are exactly that. Collecting 30 percent of another company’s in-app subscription revenue is not.</p>\n\n\n\n    "
      },
      {
         "title" : "Yours Truly on CNBC This Morning",
         "date_published" : "2021-09-15T23:39:31Z",
         "date_modified" : "2021-09-15T23:39:31Z",
         "id" : "https://daringfireball.net/linked/2021/09/15/yours-truly-on-cnbc-this-morning",
         "url" : "https://daringfireball.net/linked/2021/09/15/yours-truly-on-cnbc-this-morning",
         "external_url" : "https://www.cnbc.com/video/2021/09/15/john-gruber-apple-embracing-work-from-home-in-latest-product-line.html",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>I enjoy that I’m credited in the headline simply as “expert”. I’ll take that.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.cnbc.com/video/2021/09/15/john-gruber-apple-embracing-work-from-home-in-latest-product-line.html\">cnbc.com/video/2021/09/15/john-gruber-apple-embracing-work…</a></strong></em></p>\n"
      },
      {
         "title" : "The Old Last-Minute Hardware Design Switcheroo",
         "date_published" : "2021-09-15T16:51:55Z",
         "date_modified" : "2021-09-15T16:51:55Z",
         "id" : "https://daringfireball.net/linked/2021/09/15/old-last-minute-hardware-switcheroo",
         "url" : "https://daringfireball.net/linked/2021/09/15/old-last-minute-hardware-switcheroo",
         "external_url" : "https://www.cultofmac.com/752777/apple-watch-7-last-minute-substitution/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Killian Bell, writing at Cult of Mac:</p>\n\n<blockquote>\n  <p>Apple Watch Series 7 is not the upgrade most of us expected to see\nfrom Tuesday’s Apple event. The new model doesn’t sport the big\ndesign refresh multiple sources said was coming. It doesn’t even\npack a new chip.</p>\n\n<p>Is this the upgrade Apple wanted to deliver this year? Or is it\na last-minute substitution that Cupertino had to settle on\nbecause the refresh it really wanted to deliver just wasn’t\nready to roll out?</p>\n\n<p>Based on the evidence, we’re going to say it’s the latter.</p>\n</blockquote>\n\n<p>The only way this could be funnier is if Bell included the theory that perhaps Apple changed the hardware at the last minute <em>because</em> the flat-edge designs leaked.</p>\n\n<p>This is not how hardware works. These designs are set <em>long</em> in advance. In fact, from what I’ve heard, the flat-edge watch designs might be legitimate leaks, but they’re <em>next</em> year’s designs. That’s how far in advance Apple works on hardware — they were already in the advanced stages of designing the 2022 Apple Watches months ago. (Aesthetically, I am not sold on a flat-edge design for the watch. The round edges are iconic and organic.)</p>\n\n<p>You can argue that Series 7 is a marginal upgrade over Series 6, but with an all-new screen (brighter and bigger), all-new crystal (more durable), and 33 percent faster charging, there <em>are</em> upgrades, and none of them could be slapped together.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://www.cultofmac.com/752777/apple-watch-7-last-minute-substitution/\">cultofmac.com/752777/apple-watch-7-last-minute-substitution…</a></strong></em></p>\n"
      },
      {
         "title" : "NSO Group iMessage Zero-Click Exploit Captured in the Wild, Patched by Apple",
         "date_published" : "2021-09-15T16:20:04Z",
         "date_modified" : "2021-09-15T16:22:54Z",
         "id" : "https://daringfireball.net/linked/2021/09/15/nso-group-imessage-exploit",
         "url" : "https://daringfireball.net/linked/2021/09/15/nso-group-imessage-exploit",
         "external_url" : "https://citizenlab.ca/2021/09/forcedentry-nso-group-imessage-zero-click-exploit-captured-in-the-wild/",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p>Citizen Lab:</p>\n\n<blockquote>\n  <p>In March 2021, we examined the phone of a Saudi activist who has\nchosen to remain anonymous, and determined that they had been\nhacked with NSO Group’s Pegasus spyware. During the course of the\nanalysis we obtained an iTunes backup of the device.</p>\n\n<p>Recent re-analysis of the backup yielded several files with the\n“.gif” extension in Library/SMS/Attachments that we determined\nwere sent to the phone immediately before it was hacked with NSO\nGroup’s Pegasus spyware.</p>\n\n<p>Because the format of the files matched two types of crashes we\nhad observed on another phone when it was hacked with Pegasus, we\nsuspected that the “.gif” files might contain parts of what we are\ncalling the FORCEDENTRY exploit chain.</p>\n\n<p>Citizen Lab forwarded the artifacts to Apple on Tuesday, September\n7. On Monday, September 13, Apple confirmed that the files\nincluded a zero-day exploit against iOS and MacOS. They designated\nthe FORCEDENTRY exploit CVE-2021-30860, and describe it as\n“processing a maliciously crafted PDF may lead to arbitrary code\nexecution.”</p>\n</blockquote>\n\n<p>The files with the “.gif” extension weren’t actually GIF files — they were carefully-crafted malformed PSD and PDF files that triggered image processing bugs. What makes attacks like this particularly dastardly is that the victim apparently doesn’t even see anything. It’s invisible.</p>\n\n<p class=\"x-netnewswire-hide\" style=\"padding-top: 1.5em;\"><em>Link: <strong><a href=\"https://citizenlab.ca/2021/09/forcedentry-nso-group-imessage-zero-click-exploit-captured-in-the-wild/\">citizenlab.ca/2021/09/forcedentry-nso-group-imessage-zero…</a></strong></em></p>\n"
      },
      {
         "title" : "★ Why iPhone Names Have Numbers and Most Other Apple Product Names Don’t",
         "date_published" : "2021-09-09T18:40:15Z",
         "date_modified" : "2021-09-10T22:15:45Z",
         "id" : "https://daringfireball.net/2021/09/iphone_names",
         "url" : "https://daringfireball.net/2021/09/iphone_names",
         "authors" : [
            {
               "name" : "John Gruber"
            }
         ],
         "content_html" : "\n<p><a href=\"https://twitter.com/gruber/status/1435292384439508994\">I conducted a poll on Twitter this week</a> asking what people think the new iPhones presumably being introduced <a href=\"https://daringfireball.net/linked/2021/09/07/california-streaming-event\">next week</a> will be named. With over 4,600 votes, the results were:</p>\n\n<ul>\n<li>iPhone 13: 70%</li>\n<li>iPhone 12S: 12%</li>\n<li>iPhone (no more numbers): 15%</li>\n<li>Other: 3%</li>\n</ul>\n\n<p>I probably asked a few days too late — there was <a href=\"https://www.macrumors.com/2021/09/06/iphone-13-pro-max-silicone-cases-leak/\">a credible leak</a> purporting to show the packages for “iPhone 13 Pro Max” silicone cases from Apple over the weekend.</p>\n\n<p>What intrigued me were the number of folks responding on Twitter who said that while they voted for “iPhone 13” as what they <em>would</em> be named, they <em>wish</em> that Apple would drop the numbers and just go with <em>iPhone</em>, <em>iPhone Mini</em>, <em>iPhone Pro</em>, and <em>iPhone Pro Max</em>, with implicit model years to tell them apart from new models in subsequent years. That’s basically how Apple names its other products — with the notable exception of Apple Watch (see below).</p>\n\n<p>But just plain “iPhone” wouldn’t work for iPhones, because iPhones are different. When Apple introduces a new iPad Pro, it <em>replaces</em> the previous iPad Pro. You can’t go into an Apple Store and buy a new 2018 iPad Pro. But you <em>can</em> buy a new iPhone XR from Apple today — a model that <a href=\"https://daringfireball.net/2018/10/the_iphone_xr\">was introduced in 2018</a>. (I’d wait until <a href=\"https://daringfireball.net/linked/2021/09/07/california-streaming-event\">next Tuesday</a> before doing that.) Apple Watch is the only other product that’s sold like iPhones, with previous “series” sticking around for years at lower prices.<sup id=\"fnr1-2021-09-09\"><a href=\"#fn1-2021-09-09\">1</a></sup></p>\n\n<p>Apple wants people who are buying new iPhones that were first introduced 2–3 years ago to feel like they’re getting a new iPhone. They should, because they are — they’re great devices at lower prices, and will be supported for years to come. But if the iPhone XR were named “iPhone (2018)”, it’d feel old.</p>\n\n<p>I get it: it seems odd that in 10 years we might be awaiting the introduction of the iPhone 23 lineup, but at the moment, I don’t see this changing. <a href=\"https://www.nfl.com/videos/how-bucs-beat-chiefs-mahomes-in-super-bowl-lv-no-risk-it-no-biscuit\">The NFL just keeps counting Super Bowls</a> — at least Apple only used Roman numerals for the X and XS/XR years.</p>\n\n<div class=\"footnotes\">\n<hr />\n<ol>\n<li id=\"fn1-2021-09-09\">\n<p>The Apple Watch numbering scheme is simple: new year, new series, incremented by one. The iPhone numbering scheme is not simple. There was no iPhone 2 — the second iPhone was named iPhone 3G. Thanks to the 3GS, the iPhone 4 was in fact the fourth model year. But then came the other “S” years: 4S, 5S, 6S, XS. And Apple skipped “iPhone 9” entirely. If Apple had stuck to a numbering scheme as simple as Apple Watch’s, next week’s new iPhones would be the iPhones 15.&nbsp;<a href=\"#fnr1-2021-09-09\"  class=\"footnoteBackLink\"  title=\"Jump back to footnote 1 in the text.\">&#x21A9;&#xFE0E;</a></p>\n</li>\n</ol>\n</div>\n\n\n\n    "
      }
   ]
}







