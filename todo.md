**NOTLAR**
1. bootstrap kullanmak için: getbootstrap.com adresinden cdn linklerini base.html'e kopyalamaK yeterli. Burada iki link mevcut. İlkini base.html'de head içine, ikincisini ise yine base.html'de body'nin sonuna ekliyorum.
2. list.hmtl'de priority == önce ve sonra boşluk bırakmayınca hata verdi.Dikkat etmek lazım!!!
    {% if todo.priority == 1 %}
    <b class="text-danger">{{todo.get_priority_display}}</b> 
    {% elif  todo.priority == 2 %}
    <b class="text-warning">{{todo.get_priority_display}}</b>  
    {% else %}
    <b class="text-info">{{todo.get_priority_display}}</b> 
    {% endif %}  

3. Django kullanırken class-based kullanmak tavsiye edilir.                       
                     