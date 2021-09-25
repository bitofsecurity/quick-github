<h2>GitHub personal access token</h2>
To generate a Generate a GitHub personal access token and fix the ‘support for password authentication removed’ error, follow these steps:
<ol>
 	<li>Log into GitHub with your username and password</li>
 	<li>Navigate to your GitHub account settings</li>
 	<li>Scroll down and click ‘Developer settings’ in the list of links to the left</li>
 	<li>Click the Personal access tokens link</li>
 	<li>Click the ‘Generate new token’ button</li>
 	<li>Add a ‘Note’ to describe the tokens usage</li>
 	<li>Set an expiration date for the GitHub personal access token</li>
 	<li>Select the appropriate authentication scope</li>
 	<li>Click the ‘Generate token’ button</li>
</ol>
<h2>Quick github commands to setup</h2>
Setup username and store password
<pre>git config --global user.name myusername
git config --global user.email myemail@gmail.com
git config --global credential.helper store
</pre>
<h2>Pushing Files</h2>
<pre>git init
git add .
git commit -m 'Initial Commit' -a
</pre>
<em>Add an empty git</em>
<pre>git remote add origin https://github.com/bitofsecurity/dns-query-from-file.git
git remote -v
</pre>
<pre>git push origin master
</pre>
<h3>One file only</h3>
<pre>git commit dns-query-from-file.sh
git push origin master</pre>
<h2>Clear git history</h2>
<pre>rm -rf .git</pre>
<em>Recreate the repos from the current content only</em>
<pre>git init
git add .
git commit -m "Initial commit"</pre>
<em>push to the github remote repos ensuring you overwrite history</em>
<pre>git remote add origin https://github.com/bitofsecurity/dns-query-from-file.git
git push -u --force origin master</pre>
