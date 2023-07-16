# Angular-Blog Yönetim Sistemi Projesi

*Bu proje içerisinde yer alan içerik, tarafımızdan yapılması istenilen özellikleri dikkate alınarak geliştirilmiş olan, bir blog yönetim sistemidir.*

## Hedef
*Basit bir blog yönetim sistemi oluşturup verilerimizi eklemek, listelemek, düzenlemek ve
silmek.*

## Konu
*SQL ödevimizde hazırladığımız veritabanına uygun olarak şimdi de bu verileri
yönetebileceğimiz bir yönetim panelini Angular kullanarak tasarlamak istiyoruz. Modellerimiz
şu şekilde olacaktır.*


| User | Post |Category |Comment |
|------|------|------|------|
|userId|postId|categoryId|commentId| 
|username|userId|name|postId| 
|email|categoryId|creationDate|userId| 
|creationDate|title|    |comment|
|isActive|content|      |creationDate|
|        |viewCount|    |isConfirmed |
|        |creationDate| |            |
|        |isPublished|  |            |
    

## Önem Verdiğimiz Kriterler
1. Bileşenlerin tekrar kullanılabilirliği
2. Input, Output kullanımı
3. Servislerin oluşturulması ve component içinde inject edilmesi
4. HTML template kodu içerisinde *ngIf, *ngFor, [(ngModel)] vb. direktiflerin kullanılmış
olması
5. Sayfada istenen verileri gösterirken tercih edilebilecek Pipe kullanımları
6. Sayfada istenen verileri elde etmek için kullanılacak Javascript fonksiyonları (map,
filter, find vb.)
7. Sayfa yeniden yüklendiğinde sonradan eklenen, düzenlenen veya silinen
verilerin yok olması önemli değildir. Yalnızca ilk yüklemeden sonra istenen
verileri gerçekleştirebilmek önemlidir.

## Proje İçerisinde Kullanılan Teknolojiler
- Angular
- TypeScript
- CSS
- HTML

## Proje Sayfalarının Temel Özellikleri

- **Kullanıcı listeleme:** *Tüm kullanıcıları görebilir, yeni kullanıcı ekleyebilir, tüm kullanıcıları düzenleyebilir ve silebilirsiniz.*
- **Kategori Listeleme:** *Tüm kategorileri gösterir,kategori detaylarına erişebilir, yeni kategoriler ekleyebilir, tüm kategorileri düzenleyebilir ve kategoriye ait gönderi yoksa kategori silinebilir.*
- **Gönderi Listeleme:** *Tüm göderileri gösterir, gönderi detaylarına erişebilir,düzenleyebilir, silebilir ve yeni gönderiler ekleyebilirsiniz. Hakkında yorum yapılmış gönderileri silemezsiniz.*
- **Yorum Listeleme:** *Tüm yorumları gösterir, yeni yorumlar ekleyebilir ve silebilirsiniz.*


- **Filtreleme Özelliği:** *Her sayfa için genel filtreleme özelliği aktif edilmiştir. Sayfada yer alan içeriklere göre filtreleyebilme işlemi yapılabilmektedir.*

**Ayrıca tüm kullanıcı ve kategorilerinin; eklenirken veya düzenlenirken eşsiz olması sağlanılmıştır.**


# Projeyi Başlatma/Kurma İşlemleri

- Projeyi klonlayarak veya zip olarak indirin.
- Projeyi kullanmakta olduğunuz IDE aracılığı ile açın.
- Terminali açın
- Angular CLI yükleme için aşağıda yer alan komutu çalıştırın:
```
npm install -g @angular/cli
```
- Projeyi başlatma işlemi için gerekli olan bağımlıkları yüklemek üzere aşağıdaki kodu çalıştırın: 
```
npm install
```
veya uyumluluk sorunlarını giderek çalıştırmak için

```
npm i --legacy-peer-deps
```
- Ve projeyi başlatın ( ayağa kaldırın).

```
ng serve
```
--------------------------------------------------
--------------------------------------------------
#  Angular-Blog Management System Project
*The content in this project is a blog management system that has been developed by taking into account the features we want to make.*
## Target
*Create a simple blog management system to add, list, edit and delete our data.*
## Topic
*In accordance with the database we prepared in our SQL homework, now we will use this data
We want to design a management panel that we can manage using Angular. Our models will be as follows.*
| User | Post |Category |Comment |
|------|------|------|------|
|userId|postId|categoryId|commentId| 
|username|userId|name|postId| 
|email|categoryId|creationDate|userId| 
|creationDate|title|    |comment|
|isActive|content|      |creationDate|
|        |viewCount|    |isConfirmed |
|        |creationDate| |            |
|        |isPublished|  |            |

## Criteria We Care About
1. Reusability of components
2. Use of Input, Output
3. Creating services and injecting them in the component
4. *ngIf, *ngFor, [(ngModel)] etc. directives are used in HTML template code
to be
5. Pipe usages that can be preferred when showing the desired data on the page
6. Javascript functions to be used to obtain the desired data on the page (map,
filter, find etc.)
7. Added, edited or deleted when the page is reloaded
It does not matter if the data disappears. Only the data requested after the first upload
It is important to be able to realize the data.

## Technologies Used in the Project

- Angular
- TypeScript
- CSS
- HTML

## Key Features of Project Pages

- **User listing:** *You can see all users, add new users, edit and delete all users.*
- **Category Listing:** *Shows all categories, you can access category details, add new categories, edit all categories and if there are no posts belonging to the category, the category can be deleted.*
- **Post Listing:** *Shows all posts, you can access post details, edit, delete and add new posts. You cannot delete posts that have been commented on.*
- **Comment Listing:** *Shows all comments, you can add and delete new comments.*

- **Filtering Feature:** *General filtering feature is activated for each page. Filtering can be done according to the content on the page.*

**In addition, all users and categories are made unique when adding or editing.**


# Starting / Setting Up the Project

- Download the project as a clone or zip.
- Open the project with the IDE you are using.
- Open the terminal
- Run the command below for Angular CLI installation:
```
npm install -g @angular/cli
```
- Run the following code to install the dependencies required to initialize the project:
```
npm install
```
or compatibility issues, type the following code to run

```
npm i --legacy-peer-deps
```
- And start the project

```
ng serve
```







