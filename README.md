# avadmyofi_shvilebi

# **📃 Junior პროგრამისტის ვაკანსია Optio-ში / 2025**

## ჯორჯ ორუელის "ცხოველების ფერმა"

წარმოიდგინე ვებსაიტი, რომელიც ჯორჯ ორუელის ნაწარმოების, “ცხოველების ფერმის”, გამარტივებული ვარიანტია. საიტზე შესვლისას მომხმარებელს ხვდება შემდეგი სცენა: სხვადასხვა ცხოველები და ფრინველები, რომლებსაც აცვიათ შარვალ-კოსტიუმები, წარმოდგენილი არიან ცენტრალური ფიგურის - მთავარი ღორის, დიდი სურათის გასწვრივ. საიტის მომხმარებელს შეუძლია ინტერაქცია ამ ცხოველებთან და მთავარი ღორის სურათთან.

## **👉 შენი გამოწვევა:**

შექმენი სრული ვებ აპლიკაცია, სადაც მომხმარებელს შეუძლია:

- ინტერაქცია ცხოველებთან და ფრინველებთან.
- გაუზიაროს მათ საკვები და იხილოს მათი რეაქცია.
- დააკვირდეს ღორის სურათის ცვლილებას მათი ქმედებების ფონზე.

---

# **🧐 ტექნიკური აღწერა**

### **ფრონტ-ენდი:**

1. **მთავარი გვერდი**
    - **ცხოველების გამოსახულებები**:
        
        ცხოველების სია
        
        თითოეულ ცხოველთან მომხმარებელს შეუძლია დააჭიროს "საკვების დაყრა" ღილაკს (მაგალითად: საკენკი, ჩალა, თივა). ამ საკვებს სცენარის მიხედვით აწვდის მთავარი ღორი.
        
        საკვების დაყრისას ცხოველი მადლობას უხდის მთავარი ღორის პორტრეტს.
        
        **დამთვლელი**: თითოეული ცხოველის ქვეშ უნდა იყოს "მადლობების" მრიცხველი.
        
    - **ღორის სურათი**
        
        ღორის სურათი მდებარეობს ვებგვერდის ცენტრში.
        
        ყოველ "მადლობაზე" სურათი იცვლება (იღიმება, ბედნიერი ხდება და ა.შ.).
        
    - არააუცილებელი ფუნქცია
        - ღორის სურათზე დაკლიკებისას ის ტრიალდება და ჩნდება პუტინის სურათი.
            - ღორის სურათზე უნდა იყოს მუსიკის ჩამრთველი და ირთვებოდეს/ითიშებოდეს სიმღერა: „ჩემი საქართველო აქ არის“.
            - პუტინის სურათი: რუსეთის ჰიმნი (ან საბჭოთ სულისკვეთების რაიმე მსგავსი მელოდია)
2. **UX/UI პრინციპები**
    - სუფთა და ინტუიციური დიზაინი.
    - გამოიყენე მხოლოდ [Angular Material](https://material.angular.io/) კომპონენტები.

---

### **ბექ-ენდი:**

1. **API-ს ფუნქციონალები:**
    - **ცხოველების სია** (`GET /api/animals`):
    დააბრუნე ცხოველების სია მათი სტატუსით (მაგალითად: სახელი, მადლობების რაოდენობა).
    - **მადლობის რეგისტრაცია** (`POST /api/animals/{id}/feed`):
    განაახლ შესაბამისი ცხოველის „მადლობების“ რაოდენობა.
    დააბრუნე ღორის სურათის ცვლილების სტატუსი.
    - **ღორის სურათის ცვლილება** (`GET /api/bidzina/status`):
    დააბრუნე ღორის სურათის მიმდინარე სტატუსი (საწყისი, ბედნიერი, პუტინი).
    - **მუსიკის გადართვა** (`POST /api/music/toggle`):
    მუსიკის გადართვა ღორისა და პუტინის სცენებს შორის.
2. **მონაცემთა ბაზა:**
    - ცხოველების ცხრილი (სახელი, ტიპი, მადლობების რაოდენობა).
    - ღორის სურათის სტატუსის ცხრილი.

---

# **🛠️ გამოყენებული ტექნოლოგიები**

- **ფრონტ-ენდი:** Angular + Angular Material
- **ბექ-ენდი:** Node.js + NestJS
- **მონაცემთა ბაზა:** MongoDB ან PostgreSQL
- **მუსიკის პლეიერი:** Web Audio API

---

# **🔥 ბონუსი**

- **NGRX-ს გამოყენება სთეითის მართვისთვის.**
- **Unit Test-ები.**
- **Data View - სურთების ნაცვლად გამოჩნდება დეტალური ცხრილი, სორტირებისა და ფილტრაციის ფუნქციებით**

---

# 🏢 ოპტიოს შესახებ

Optio ერთ-ერთი წამყვანი ქართული სტარტაპია, რომელიც ქმნის კომპლექსურ ტექნოლოგიურ პროდუქტს საშუალო და დიდი ზომის კომპანიებისთვის ფინანსურ სექტორში. ჩვენი უახლესი Customer Data Platform (CDP) კომპანიებს საშუალებას აძლევს სწრაფად და ეფექტურად გააანალიზონ თავიანთი მომხმარებლების მონაცემები და აწარმოონ პერსონალიზებული მარკეტინგული კომუნიკაცია, როგორც ციფრულ, ასევე პირდაპირ საკომუნიკაციო არხებში.

ამ მიზნის მისაღწევად ვიყენებთ მოწინავე ტექნოლოგიებს, როგორიცაა Big Data, Machine Learning, NLP, Microservice Architecture, Business Process Automation, Data Enrichment და სხვა.

ჩვენი ტექნოლოგიური სტეკი მოიცავს: Angular, Node.js, Python, Elasticsearch, Redis, RabbitMQ. საჭიროების შემთხვევაში ვმუშაობთ MS SQL, Oracle, MongoDB, .NET Core და მრავალ სხვა სისტემასთან ინტეგრაციაზე.

### დამატებით
ჩვენს გუნდში უკვე არიან როგორც დამწყები, ასევე საშუალო და მრავალწლიანი გამოცდილების მქონე პროგრამისტები. მათ ყავთ საქართველოში ერთ-ერთი საუკეთესო მენტორი, რომელიც უზრუნველყოფს შენს პროფესიულ განვითარებას და დაგეხმარება შეისწავლო:

- სწორი მიდგომები Javascript/Typescript/Angular/NodeJS ენების და ტექნოლოგიების გამოყენებით;
- Clean code-ის სტანდარტები;
- Git-თან მუშაობის საუკეთესო პრაქტიკა;
- კომპლექსური სისტემების არქიტექტურა;
- გუნდური მუშაობა;
- ავტომატური ტესტირება.

---

# ⚖️ შეფასების კრიტერიუმები

ჩვენ ვეძებთ ახალგაზრდებს, რომლებსაც უკვე აქვთ მინიმუმ ექვს თვიანი რეალური სამუშაო გამოცდილება და გადაწყვიტეს, რომ პროფესიული ცოდნა კომპლექსური ციფრული პროდუქის შექმნით გაიღრმავონ. 

ამოცანის შეფასებისას ყურადღებას მივაქცევთ:
- შინაარსის გააზრება
- ტექნიკური გადაწყვეტა
- მოთხოვნების დაფარვა
- კოდის ხარისხი
- ოპტიმალური ალგორითმები

> რჩევა: ნუ დაუთმობთ მნიშვნელოვან დროს ვიზუალურ ეფექტებსა და სურათების ხარისხს

ჩვენთვის მნიშვნელოვანია, ვიპოვოთ ცნობისმოყვარე, სწავლასა და შრომაზე ორიენტირებული ადამიანები, რომლებიც Optio-ში მუშაობის დაწყებიდან მალევე, სრული დატვირთვით ჩაერთვებიან პროექტებში.

# 🗓️ Optio-ში დასაქმების პროცესი
1. კანდიდატების მიერ შესრულებული სამუშაოს გამოგზავნა - 7 თებერვლამდე
2. შესრულებული სამუშაოების შეფასება და ონლაინ ინტერვიურერების გამოვლენა - 15 თებერვლამდე
3. პირისპირ გასაუბრების კანდიდატების შერჩევა - 20 თებერვლამდე
4. შეთავაზება - 25 თებერვლამდე
5. სამ თვიანი გამოსაცდელი პერიოდი
6. სრულყოფილი დასაქმება Optio-ში


# 📧 დავალების მოწოდება
- შესრულებული ამოცანა ატვირთე GitHub-ზე და რეპოზიტორის ლინკი გამოგვიგზავნე ელფოსტაზე [hr@optio.ai](mailto:hr@optio.ai) სათაურით `Optio Junior Software Engineer 2025 - ${YOUR_NAME_HERE}`.
- შესრულების ვადა: 07.02.2025.

---

# **🎉 წარმატებები! 🎉**
