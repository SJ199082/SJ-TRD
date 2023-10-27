# SJ-TRD.COM
My dear friends, I have a question regarding my website, which was designed using PHP. I'm currently trying to change the URL of a specific page from:
www.sj-trd.com/index.php?page=show&ex=2&dir=docs&lang=2&ser=1&cat=70&act=70&
to:
www.sj-trd.com/company-exhibition or www.sj-trd.com/blog
I've attempted to modify the .htaccess file and used the following code:
RewriteEngine On RewriteCond %{HTTPS} !=on RewriteRule ^ https://%{HTTP_HOST}%{REQUEST_URI} [L,R=301] RewriteRule ^index.php?page=show&ex=2&dir=docs&lang=2&ser=1&cat=70&act=70&$ https://sj-trd.com/blog [L,R=301]
However, no changes have occurred, and the target page hasn't changed as required. Does anyone have any ideas or solutions for this issue?
