---
title: "TryHackMe Brookly Nine Nine WriteUp"
header:
 
categories:
   - CTF
   - TryHackMe
tag:
   -TryHackMe
---

Selamlar bu yazımda TryHackMe'de bulunan Brookly Nine Nine makinesinin çözümünden bahsedeceğim. Umarım öğretici bir yazı olur, keyifli okumalar.

## Nmap 

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/Brookly_Nine_Nine/1.png){: .align-center}

80 Portu ziyaret edildikten sonra kaynak kodu incelendiğinde bir ipucu bulunmaktadır. "Have you ever heard of steganography?"

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/Brookly_Nine_Nine/2.png){: .align-center}

Web sayfasında bulunan görsel indirilip stegcracker ile incelenmektedir.

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/Brookly_Nine_Nine/3.png){: .align-center}

Holt kullanıcısının parolası elde edilmektedir.

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/Brookly_Nine_Nine/4.png){: .align-center}

Tespit edilen bilgiler ile SSH bağlantısı sağlanmaktadır ve user.txt elde edilmektedir.

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/Brookly_Nine_Nine/5.png){: .align-center}

"sudo -l" komutu ile nano'nun sudo yetkileri ile çalıştığı gözlemlenmektedir. GTFOBins aracılığıyla root yetkileri elde edilmektedir.

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/Brookly_Nine_Nine/6.png){: .align-center}

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/Brookly_Nine_Nine/7.png){: .align-center}

Root yetkileri elde edildikten sonra root.txt elde edilmektedir.

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/Brookly_Nine_Nine/8.png){: .align-center}





