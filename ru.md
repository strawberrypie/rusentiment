
# Sentiment annotation
In sentiment analysis, our goal is to isolate the feeling or attitude being conveyed through a post on social media. Some posts express an obvious positive or negative sentiment or attitude towards something, and we need to select such clear, unambiguous cases. 

The sentiment conveyed in text may refer to (1) the speaker’s subjective mood, feeling, or emotion, or to (2) the speaker’s attitude towards something.  For example:

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
</style>
<table class="tg">
  <tr>
    <th class="tg-031e">(1) Speaker mood/emotions</th>
    <th class="tg-031e">(2) Evaluation of an entity or event</th>
  </tr>
  <tr>
    <td class="tg-031e">I am so excited!</td>
    <td class="tg-031e">Princess and the frog is a great movie</td>
  </tr>
  <tr>
    <td class="tg-031e">I am happy</td>
    <td class="tg-031e">Our Country is doing great</td>
  </tr>
</table>

Both the speaker’s mood and their attitude towards something can be positive or negative:



<table class="tg" style="width: 652px;">
<tbody>
<tr>
<th class="tg-031e" style="width: 182px;">&nbsp;</th>
<th class="tg-031e" style="width: 227px;">Positive</th>
<th class="tg-031e" style="width: 233px;">Negative</th>
</tr>
<tr>
<td class="tg-031e" style="width: 182px;">Emotions, mood of the speaker</td>
<td class="tg-031e" style="width: 227px;">
<p>happiness, pride, love, inspiration, serenity, interest&hellip;</p>
<ul>
<li>I am proud of my work</li>
<li>Really pleased to announce their engagement...</li>
<li>So excited. Yay!</li>
</ul>
</td>
<td class="tg-031e" style="width: 233px;">
<p>sadness, anger, fear, hatred, pain, disgust, shame, guilt&hellip;</p>
<ul>
<li>I am so tired of waking up sad in the morning</li>
<li>I am mad as hell for way too many reasons</li>
</ul>
</td>
</tr>
<tr>
<td class="tg-031e" style="width: 182px;">Evaluation, attitude towards some entity or event</td>
<td class="tg-031e" style="width: 227px;">
<ul>
<li>I'm looking forward to next year's July event</li>
<li>I like the kind of people who get excited about the stars at night</li>
<li>people who keep their word are real</li>
</ul>
</td>
<td class="tg-031e" style="width: 233px;">
<ul>
<li>I am literally disgusted at the crowd</li>
<li>Yes, you are racist, sexist, homophobic, and xenophobic if I find out you voted for Trump.</li>
</ul>
</td>
</tr>
</tbody>
</table>

All of the above cases (whether they deal with the speaker’s emotions/mood or evaluation/attitude) are cases of explicit sentiment - you can tell the sentiment because it is clearly stated in the post. However, in many cases the sentiment may be implicit - you can understand how the speaker feels or what his/her attitude towards something is, but it is not expressed directly. Cases of implicit sentiment include: 

<table class="tg" style="width: 637px;">
<tbody>
<tr>
<th class="tg-l711" style="width: 137px;">&nbsp;</th>
<th class="tg-l711" style="width: 229px;">Positive</th>
<th class="tg-l711" style="width: 259px;">Negative</th>
</tr>
<tr>
<td class="tg-l711" style="width: 137px;">Wishing (or not) for something, recommendations<br /><br />EVALUATION IS IMPLIED</td>
<td class="tg-l711" style="width: 229px;"><br />
<ul>
<li>Definitely follow these bloggers in 2018</li>
<li>You should have a functional brain, an enduring spirit and a praying tongue</li>
<li>Try the keto diet</li>
</ul>
</td>
<td class="tg-l711" style="width: 259px;">
<ul>
<li>THIS! MUST! STOP!!</li>
<li>Enough, hyping up our news</li>
<li>No one should have to go through this</li>
<li>I wouldn't wish that on a dog.</li>
</ul>
</td>
</tr>
<tr>
<td class="tg-l711" style="width: 137px;">Descriptions of experience that most people would consider positive or negative<br /><br />EMOTION IS IMPLIED</td>
<td class="tg-l711" style="width: 229px;">
<ul>
<li>We won! All the love Sometimes it only takes a sunset to make you realize that life is still worth living after all</li>
<li>I got promoted to assistant manager yaaaasToday, my beautiful #bestie beat cancer&rsquo;s ass!</li>
</ul>
</td>
<td class="tg-l711" style="width: 259px;">
<ul>
<li>My favourite grandparent is dying, my parent might have cancer, a close friend is at a bad place mentally and I just lost my most cherished job- things have been very tough.</li>
<li>This is the heartbreaking reality of @realDonaldTrump&rsquo;s barbaric family separation policy. This must end. And it must end immediately.</li>
<li>I&rsquo;m watching Anthony Bourdain: Parts Unknown and, realize that someone like him is actually gone.</li>
</ul>
</td>
</tr>
<tr>
<td class="tg-l711" style="width: 137px;">Questions with clear implicit sentiment (often rhetorical)<br /><br />EMOTION is IMPLIED</td>
<td class="tg-l711" style="width: 229px;">&nbsp;</td>
<td class="tg-l711" style="width: 259px;">
<ul>
<li>Hmm How can I fix this now???</li>
<li>I don't understand how this keeps happening</li>
<li>How am I always late to everything??</li>
</ul>
</td>
</tr>
</tbody>
</table>

Unfortunately, it is not always the case that a whole single post fits one of the above categories. If the post contains several expressions of sentiment, we ask you to annotate the polarity of the post as a whole, which we define as the dominant, prevailing sentiment. Annotation of the mixed sentiment posts (such as the posts containing both positive and negative sentiment) is discussed in more detail on p. 7.

Posts may express sentiment of two different types, for example, the speaker's mood and the speaker's attitude towards something.  The polarity of these may be the same or it may differ, creating a mixed-sentiment post.  Often, the polarity will be the same.  For example, “Great! I won a free ticket!” has both an explicit evaluation of the event (Great!) and describes the experience that would be positive for many people (won free ticket). It is clear that the polarity of the post as a whole is also positive. 

##  Positive speech acts 
A large portion of posts express perform the functions of various speech acts: expressing gratitude for something, congratulating a user or a group of users, greeting them. We treat these as a separate subcategory because, although generally greetings, congratulations and gratitude imply positive sentiment, they can also be performed, e.g., out of a feeling of obligation or under social pressure. So we would like to keep it an option to add or remove them in different research scenarios.

This group includes: 

**Expressions of gratitude:**
- Thank you to everyone for the birthday wishes too  I appreciate all of your messages! 
- Special thanks to our mentors, Mr. Robert Lim and Ms. Arbie Belmonte. 
- I appreciate how far we have come  

**Congratulations:**
- Wish u happy bday macha.. live and be happy... 
- Happy 13 years anniversary to the cutest couple in the World!!! 
- Happy 4th of July guys! Here is my gift to you today!

**Good wishes to someone:**
- Good luck to you in your new adventure, Jack. You deserve it!
- Kind regards and best wishes from Checkpoint Charlie

**Greetings:**
- Good morning everyone! How are you doing today?
- Heyy girl ! long time no see..
- What’s up!. how have you been?

If there is clear irony, treat these as cases of mixed sentiment (see page 7).

## Posts that dont express sentiment

No sentiment” label is reserved for posts that simply describe some situation in a neutral, matter-of-fact way, and have no clear positive or negative sentiment. For example:

- my friend is coming down from Indiana today to see your show tonight <span style="float:right;"> [no sentiment]</span>
- 18 new friend requests  <span style="float:right;"> [no sentiment]</span>
- french toast, bacon, and scrambled egg <span style="float:right;"> [no sentiment]</span>

The same label applies to most matter-of-fact, non-rhetorical questions:
- Now, my friends, are you coming with me? <span style="float:right;"> [no sentiment]</span>
- Where did you put my keys? <span style="float:right;"> [no sentiment]</span>
- So, what's new? <span style="float:right;"> [no sentiment]</span>

If the post carries no overall sentiment, but is followed by smileys, please use the “no sentiment” label. For example:
 - I am back online:)))😝 <span style="float:right;"> [no sentiment]</span>
 - Here is some actual data 😅😍 <span style="float:right;"> [no sentiment]</span>

Other categories of posts that should be annotated with “no sentiment” label include:

**(1) Advertisements:**
- Free, confidential & friendly advice for people living in Central Bedfordshire. Try AdviceCentral for help on a wide range of topics. <span style="float:right;"> [no sentiment]</span>
- We are looking for a Graphic Designer! Immediate position, in office only - no freelance. Come join us for our annual Open House this Saturday, July 14th! Lot of great hand-on opportunities for kids and adults! <span style="float:right;"> [no sentiment]</span>
- My yacht is officially for sale. Highest bidder by Friday gets it <span style="float:right;"> [no sentiment]</span>

**(2) Professional plot summaries of movies, books, etc:**
- The first Deadpool remains one of my very favorite superhero movies and the sequel at least from what we've seen appears to retain the same humorous spirit that made the original so great. <span style="float:right;"> [no sentiment]</span>

- "What Happened” is not one book, but many. It is a candid and blackly funny account of her mood in the direct aftermath of losing to Donald J. Trump. <span style="float:right;"> [no sentiment]</span>

**(3) Requests for information:**

- Do you sell those knife rolls or will I have to get one from amazon? <span style="float:right;"> [no sentiment]</span>
- How quick can you deliver one to me? <span style="float:right;"> [no sentiment]</span>
- Where will store be and when will you open? DM me please. <span style="float:right;"> [no sentiment]</span>

Neutral posts do not necessarily contain full clauses. For instance, they may be titles or descriptions of media or files attached to а post:

- Moved to room 3 <span style="float:right;"> [no sentiment]</span>
- Test Prep In-Home Tutors in New Hampshire <span style="float:right;"> [no sentiment]</span>
- Weather in 10 days <span style="float:right;"> [no sentiment]</span>

# Smileys

An important caveat concerns smileys. We distinguish 3 cases:
1. smileys are the ONLY indication of any sentiment.
 No need to help <span style="float:right;"> [no sentiment]</span>
 we are hiring! :) <span style="float:right;"> [no sentiment]</span>

Such posts should be annotated with the “no sentiment” label, because the smileys here are used to simply mimic the facial expressions in a normal face-to-face conversation rather than express strong sentiment. Besides, they are easy to detect automatically

2. smileys MIRROR the sentiment expressed verbally:
That steak was outta control. I am in a food coma:)))<span style="float:right;"> [no sentiment]</span>
bday dinner was nothing short of awesome 😍😍 and my baby looked GREAT 😜<span style="float:right;"> [no sentiment]</span>
I have job interview. I am a nervous wreck   <span style="float:right;"> [no sentiment]</span>

Such posts should be annotated to reflect the sentiment expressed verbally.
3. smileys CHANGE the sentiment expressed verbally:
BAD BOY:))))))<span style="float:right;"> [no sentiment]</span>
What an AWFUL way to lose the game Oakland 😂😂😂<span style="float:right;"> [no sentiment]</span>

In such cases the overall dominant sentiment should be annotated. The smileys weaken the explicit negative evaluation in bad/awful, they indicate that the speaker is joking. The overall sentiment is positive - although it is only expressed by the smileys.

4. smileys HEDGE the overall sentiment, usually serving to make negative sentiment sound slightly less negative, but not completely reversing the sentiment.
I'm so grumpy. The drink I ordered from @Starbucks looks and tastes like a cup of cream. Fail:)))<span style="float:right;"> [no sentiment]</span>
Car broke down this morning, what an awful way to start my day:)))<span style="float:right;"> [no sentiment]</span>

In these examples, the smileys weaken the explicit negative evaluation, but the overall sentiment is still negative. 

5. Unlike smileys, words indicating mood (laughter, cries, swearing etc.) should always be taken into account. 

 LOL stop judging my spelling, its beautiful HAHAHA <span style="float:right;"> [no sentiment]</span>
We had a good tournament, but fuuuck me. What a terrible way to go out. FML<span style="float:right;"> [no sentiment]</span>

Abbreviations like LOL and OMG should also be taken into account.






bla bla bla <span style="float:right;"> [no sentiment]</span>



