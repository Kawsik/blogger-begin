```xhtml
<!-- My Practice START |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||| -->
<div style='background: #fff; min-height: 181px; font-size: 1.7em;'>
<!-- My Practice START |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||| -->


  <b:if cond='data:blog.pageType == "item"'>
    <p>This is post page:
      <br/>
		any post page - yes.
		
		</p>
  </b:if>


  <b:if cond='data:blog.pageType == "static_page"'>
      <p>This is Static page:
        <br/>
		any page page - yes
		</p>
  </b:if>


  <b:if cond='data:blog.pageType == "index"'>
    <p>This is Home or post list:
      <br/>
		home page - yes
      <br/>
		post list page via clicking Year Name only on archieve - yes
      <br/>
		post list page via clicking a label - yes
      <br/>
		post list page via searching - yes
		</p>
  </b:if>


  <b:if cond='data:blog.url == data:blog.homepageUrl'>
    <p>This is Home Page:
      <br/>
		home page - yes
	</p>
  </b:if>


  <b:if cond='data:blog.url == "http://khelaghor-practice.blogspot.com/search/label/Label%20ONE"'>
	<p>showing with specific link: - yes - /search/label/Label%20ONE</p>
  </b:if>
  <b:if cond='data:blog.url == "http://khelaghor-practice.blogspot.com/"'>
	<p>showing with specific link: - yes - home</p>
  </b:if>
  <b:if cond='data:blog.url == "http://khelaghor-practice.blogspot.com/2017/03/demo-post-three.html"'>
	<p>showing with specific link: - yes - /2017/03/demo-post-three.html</p>
  </b:if>
  <b:if cond='data:blog.url == "http://khelaghor-practice.blogspot.com/p/demo-four.html"'>
	<p>showing with specific link: - yes - /p/demo-four.html</p>
  </b:if>
  <b:if cond='data:blog.url == "http://khelaghor-practice.blogspot.com/2017_03_01_archive.html"'>
	<p>showing with specific link: - no - /2017_03_01_archive.html</p>
  </b:if>
  <b:if cond='data:blog.url == "http://khelaghor-practice.blogspot.com/search?updated-min=2017-01-01T00:00:00-08:00"'>
	<p>showing with specific link: - unknown - /search?updated-min=2017-01-01T00:00:00-08:00</p>
  </b:if>
  <b:if cond='data:blog.url == "http://khelaghor-practice.blogspot.com/search?q=demo"'>
	<p>showing with specific link: - unknown - /search?q=demo</p>
  </b:if>


  <b:if cond='data:blog.pageType == "error_page"'>
    <p> This is Error Page:
      <br/>
		error page - yes
	</p>
  </b:if>


  <b:if cond='data:post.showBacklinks'>
	<p>showing backlink ? I dont know</p>
  </b:if>


  <b:if cond='data:displayname == "specific-name"'>
	<p>showing when matching display name ? I dont know</p>
  </b:if>


  <b:if cond='data:post.numComments == [number_here]'>
	<p>showing when matching display name ? I dont know</p>
  </b:if>


  <b:if cond='data:post.hasJumpLink'>
	<p>showing when matching display name ? I dont know</p>
  </b:if>


  <b:if cond='data:post.allowComments'>
	<p>showing when matching display name ? I dont know</p>
  </b:if>





<!-- My Practice END |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||| -->
</div>
<!-- My Practice END |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||| -->
```
