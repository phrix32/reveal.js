# Gitflow
A successful Git branching model
---
## Main branches
---
<section data-background-image="images/main-branches.png" data-background-size="contain"></section>
<section>
  <h3>Master branch</h3>
  <ul>
    <li>Always reflects a <i>production-ready</i> state</li>
    <li>Tagged with release numbers</li>
  </ul>
  <h4><i>Production</i> deployment branch</h4>
</section>
<section>
  <h3>Develop branch</h3>
  <ul>
    <li>Branch off from master</li>
    <li>Nightly builds are built from this branch</li>
  </ul>
  <h4><i>Devbox</i>, <i>Deploy</i> and <i>Latest</i> deployment branch</h4>
</section>
---
## Supporting branches
---
<section>
  <h3>Feature branch</h3>
</section>

<section data-background-image="images/branch-feature.png" data-background-size="contain"></section>

<section>
  <table>
    <tr>
      <td>May branch off from</td>
      <td><i>develop</i></td>
    </tr>

    <tr>
      <td>Must merge back into</td>
      <td><i>develop</i></td>
    </tr>

    <tr>
      <td>Branch naming convention</td>
      <td>anything except <i>master</i>, <i>develop</i>, <i>release/*</i>, or <i>hotfix/*</i></td>
    </tr>
  </table>
</section>
---
<section>
  <h3>Hotfix branch</h3>
</section>

<section data-background-image="images/branch-hotfix.png" data-background-size="contain"></section>

<section>
  <table>
    <tr>
      <td>May branch off from</td>
      <td><i>master</i></td>
    </tr>

    <tr>
      <td>Must merge back into</td>
      <td><i>master</i> and <i>develop</i></td>
    </tr>

    <tr>
      <td>Branch naming convention</td>
      <td>hotfix/*</td>
    </tr>
  </table>
</section>
---

<section>
  <h3>Release branch</h3>
</section>

<section data-background-image="images/branch-release.png" data-background-size="contain"></section>

<section>
  <table>
    <tr>
      <td>May branch off from</td>
      <td><i>develop</i></td>
    </tr>

    <tr>
      <td>Must merge back into</td>
      <td><i>develop</i> and <i>master</i></td>
    </tr>

    <tr>
      <td>Branch naming convention</td>
      <td>release/*</td>
    </tr>
  </table>
</section>

<section>
  <h4><i>Staging</i> deployment branch</h4>
</section>
---
<section>
    <h2>Overall view</h2>
</section>

<section data-background-image="images/overview.png" data-background-size="contain">
</section>
---
## Misc
* Small changes (1 commit) can be done in dev branch directly
* Same for fixes of already merged features
---
## Git commands you'll need
* git checkout -b [branch-name]
* git merge -no-ff [branch-name]
* git branch -d [branch-name]
* git tag -a [tag-name]
* obviously git clone, commit and push
---
<h2>Links</h2>
<section>
    <h3>Reading</h3>
    <ul>
        <li>https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow</li>
        <li>http://nvie.com/posts/a-successful-git-branching-model/</li>
        <li>http://danielkummer.github.io/git-flow-cheatsheet/</li>
    </ul>
</section>
<section>
    <h3>Video</h3>
    <ul>
        <li>http://vimeo.com/16018419</li>
        <li>https://buildamodule.com/video/change-management-and-version-control-deploying-releases-features-and-fixes-with-git-how-to-use-a-scalable-git-branching-model-called-gitflow</li>
    </ul>
</section>
<section data-markdown>
    <h3>Tools</h2>
    <ul>
        <li>https://github.com/nvie/gitflow</li>
    </ul>
</section>
