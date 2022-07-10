[![Codacy Badge](https://api.codacy.com/project/badge/Grade/294403aef0f4418f86d43639425d6262)](https://www.codacy.com/manual/amirbagh75/ansible-masshadlug?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=amirbagh75/ansible-masshadlug&amp;utm_campaign=Badge_Grade)
<div dir='auto'>
<h2> ارائه Ansible مشهدلاگ </h1>
</div>

<div dir='rtl'>

Ansible چیست؟

انسیبل یا Ansible را اصطلاحا software provisioning, configuration management و application-deployment tool مینامند. خودمونی ترش این میشه که با Ansible میشه خیلی راحت تر تعداد زیاد سرور یا حتی ۱ عدد سرور رو مدیریت کرد. مثلا یکبار برای همیشه نصب اصولی nginx رو یاد بگیریم و با ansible پیاده کنیم و همیشه و همه جا ازش استفاده کنیم. یا مثلا میتونیم باهاش روی ۱۰ تا سرور شرکت چک کنیم اگر نسخه کرنل زیر فلان بود به مدیرسیستم ها خبر بده که فلان کار را بکنند یا حتی خودش یک کاری رو بکنه. معماری انسیبل را اصطلاحا pull configuration مینامند. معنیش اینه که یک سرور مرکزی وجود داره که به بقیه خبر میده که چه کار بکنن. البته میشه ansible رو روی حالت push configuration هم استفاده کرد. یعنی یک عالمه سرور از یک جایی دستورات رو میگیرن و سعی میکنن خودشونو شبیه اون خواسته دستورات بکنند. هر کدوم خوبی ها و بدی های خودشو داره. توی ارائه من درباره همه این ها صحبت کردم. لینک PDF ارائه رو میتونید از [اینجا](https://github.com/amirbagh75/ansible-masshadlug/blob/master/ansible.pdf) دانلود بکنید. 

مستندات Ansible خیلی زیاده و خیلی کامل ولی اگر بخوام تیتروار بهشون برسیم من یک سری چیزای خوبشو اینجا گردآوری کردم:

-  [نصب کردن روی اوبونتو](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#latest-releases-via-apt-ubuntu)
-  [مواد تشکیل دهنده Ansible](https://docs.ansible.com/ansible/latest/user_guide/basic_concepts.html)
-  [Inventory یا همان سرورها در Ansible](https://docs.ansible.com/ansible/latest/user_guide/intro_inventory.html)
-  [اجرا کردن کامند ها بدون Playbook ها به صورت ad-hoc](https://docs.ansible.com/ansible/latest/user_guide/intro_adhoc.html)
-  [درک مفاهیم اولیه Playbook ها](https://docs.ansible.com/ansible/latest/user_guide/playbooks_intro.html#playbooks-intro)
-  [نوشتن Playbook های چندبار مصرف (DRY)](https://docs.ansible.com/ansible/latest/user_guide/playbooks_reuse.html)
-  [Bestpractice هایی برای نوشتن Playbook](https://docs.ansible.com/ansible/latest/user_guide/playbooks_best_practices.html)
-  [لیست Module های موجود در Ansible و تنظیماتشون](https://docs.ansible.com/ansible/latest/user_guide/modules.html)


مثال هایی از Ansible CLI:

<div dir='ltr'>

-  <code>ansible localhost -m ping</code>
-  <code>ansible -i hosts.ini all -m shell -a 'uname -s -r'</code>
-  <code>ansible -i hosts.ini all -m setup</code>
-  <code>ansible-inventory -i hosts.ini --list</code>
-  <code>ansible-inventory -i hosts.ini --graph</code>
-  <code>ansible-playbook install.yaml -K</code>
-  <code>ansible-playbook install.yaml -K --tags "update_ui"</code>
-  <code>ansible-doc --list</code>
-  <code>ansible-doc ufw</code>

</div>

</div>
