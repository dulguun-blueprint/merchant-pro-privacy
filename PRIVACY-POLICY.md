# Нууцлалын бодлого — Blueprint Merchant

> **Ноорог.** Нийтлэхээс өмнө хуульчаар хянуулж, `{{…}}` гэсэн бүх хэсгийг бөглөнө. Энэ баримт аппын 1-р хувилбарын (v1) бодит ажиллагаанд тулгуурласан: апп шинэ төрлийн мэдээлэл цуглуулж эхлэх бүрт (жишээ нь push мэдэгдэл, алдааны тайлан, камер) энд нэмж шинэчилнэ.

**Хүчин төгөлдөр болсон огноо:** {{YYYY-MM-DD}}

## 1. Бид хэн бэ

Blueprint Merchant аппыг {{Блүпринт Солюшнс ХХК-ийн бүтэн албан ёсны нэр}} (цаашид «Blueprint», «бид») хөгжүүлж ажиллуулдаг. Хаяг: {{хаяг}}. Холбоо барих: {{имэйл}}, {{утас}}.

Апп нь дэлгүүр, байгууллагын ажилтан өөрийн байгууллагыг харилцагчаар бүртгэсэн нийлүүлэгчдээс бараа захиалахад зориулагдсан. Аппыг ажилтан өөрийн байгууллагын нэрийн өмнөөс ашиглана.

Хувь хүний мэдээллийг Монгол Улсын Хүний хувийн мэдээлэл хамгаалах тухай хууль болон холбогдох бусад хууль тогтоомжийн дагуу боловсруулна.

## 2. Ямар мэдээлэл цуглуулдаг вэ

**Нэвтрэх бүртгэл (BP ID).** Апп руу BP ID бүртгэлээр нэвтэрнэ. Нууц үгийг BP ID-ийн хуудсанд оруулдаг бөгөөд апп нууц үгийг хэзээ ч харахгүй, хадгалахгүй. Нэвтрэхэд BP ID апп руу таны нэр, утасны дугаар, имэйл хаяг болон бүртгэлийн дугаарыг дамжуулна.

**Байгууллага, салбар.** Таны ажилладаг байгууллагын нэр, регистрийн дугаар, таны хуваарилагдсан салбаруудын нэр, хаяг, утас. Энэ мэдээллийг танай байгууллагын админ бүртгэдэг.

**Захиалга.** Таны сагсанд хийсэн бараа, тоо хэмжээ, илгээсэн захиалга, хүргүүлэх өдөр, захиалгад бичсэн тэмдэглэл, захиалгын төлөв, хүргэлтийн мэдээлэл.

**Техникийн мэдээлэл.** Сервер рүү хандах бүрт хүсэлтийн дугаар, хандсан цаг зэрэг үйлчилгээг ажиллуулахад шаардлагатай бүртгэл (log) үүснэ.

**Бид цуглуулдаггүй:** байршил, харилцагчдын жагсаалт, зураг, камер, микрофон, санхүүгийн карт, сурталчилгааны танигч. Апп сурталчилгаа харуулахгүй, таныг бусад апп, вэбсайтаар дагаж мөрдөхгүй.

## 3. Мэдээллийг юунд ашигладаг вэ

- Таныг таньж нэвтрүүлэх, таны байгууллага, салбарыг тодорхойлох;
- Таны байгууллагын гэрээт нийлүүлэгчдийн бараа, гэрээний үнийг харуулах;
- Таны илгээсэн захиалгыг нийлүүлэгч рүү дамжуулж, явцыг харуулах;
- Алдааг шалгаж засах, үйлчилгээний аюулгүй байдлыг хангах.

Бид таны мэдээллийг худалдахгүй, сурталчилгаанд ашиглахгүй.

## 4. Хэнтэй хуваалцдаг вэ

**Нийлүүлэгч.** Захиалга илгээхэд тухайн нийлүүлэгч захиалгын мөрүүд, хүргэх салбарын нэр, хаяг, утас, хүргүүлэх өдөр, тэмдэглэлийг хүлээн авна. Нийлүүлэгч танай байгууллагын бусад салбарын жагсаалтыг харахгүй.

**Таны байгууллага.** Танай байгууллагын эрх бүхий ажилтнууд байгууллагынхаа нэрийн өмнөөс өгсөн захиалгыг харах боломжтой.

**Үйлчилгээ үзүүлэгч.** Сервер байршуулах ({{hosting үйлчилгээ үзүүлэгч, улс}}) зэрэг бидний өмнөөс ажилладаг гүйцэтгэгчид зөвхөн бидний зааврын дагуу мэдээлэлд хандана.

**Хууль.** Хуульд заасан үндэслэлээр эрх бүхий байгууллага шаардсан тохиолдолд.

## 5. Таны утсанд юу хадгалагддаг вэ

- **Нэвтрэх токен** — утасны хамгаалалттай сан (iOS Keychain, Android Keystore)-д;
- **Сагс, сонгосон салбар** — таныг дахин нээхэд сагс хэвээр үлдэхийн тулд;
- **Барааны мэдээллийн нөөц** (нэр, код, баркод) — хайлтыг хурдан, сүлжээгүй үед ч ажиллуулахын тулд. Үнэ, үлдэгдлийг нөөцлөхгүй.

Эдгээр нь танай бүртгэл, байгууллага тус бүрээр тусгаарлагдсан. **Апп-аас гарахад** (Бүртгэл → Гарах) утсан дээрх таны бүх мэдээлэл устана. Аппыг устгахад мөн адил.

## 6. Хэр удаан хадгалдаг вэ

- Захиалгын мэдээллийг нийлүүлэгч ба танай байгууллагын нягтлан бодох бүртгэлийн шаардлагын дагуу {{хугацаа, жишээ нь хуулиар шаардсан хугацаа}} хадгална.
- Серверийн техникийн бүртгэлийг {{хугацаа}} хадгалаад устгана.
- Таны BP ID бүртгэлийн мэдээллийг BP ID-ийн нууцлалын бодлогын дагуу хадгална: {{BP ID-ийн нууцлалын бодлогын холбоос}}.

## 7. Аюулгүй байдал

Апп болон серверийн хоорондох бүх холболт шифрлэгдсэн (HTTPS). Нэвтрэх токен утасны хамгаалалттай санд хадгалагдана. Сервер таны байгууллага, салбарын эрхийг хүсэлт бүр дээр шалгадаг тул та өөр байгууллага, өөр салбарын мэдээлэлд хандах боломжгүй.

## 8. Таны эрх

Та өөрийн мэдээллийг харах, засуулах, устгуулах, боловсруулахыг эсэргүүцэх эрхтэй. Хүсэлтээ {{имэйл}} хаягаар илгээнэ үү; бид {{хоног}} хоногт багтаан хариулна.

Таны нэр, утас, байгууллага, салбарын мэдээллийг танай байгууллагын админ бүртгэдэг тул засварыг эхлээд админдаа хандаж хийлгэнэ үү. Нийлүүлэгчид илгээгдсэн захиалгыг нийлүүлэгч өөрийн бүртгэлд хуулийн дагуу хадгалж болно.

**Бүртгэл устгах:** {{устгах хүсэлт гаргах арга — имэйл эсвэл вэб хуудас. Google Play болон App Store үүнийг шаарддаг.}}

## 9. Хүүхэд

Апп нь байгууллагын ажилтанд зориулагдсан бөгөөд 18 нас хүрээгүй хүнд зориулагдаагүй.

## 10. Өөрчлөлт

Энэ бодлогыг өөрчлөх тохиолдолд шинэ хувилбарыг энд нийтэлж, хүчин төгөлдөр болох огноог шинэчилнэ. Томоохон өөрчлөлтийг апп дотор мэдэгдэнэ.

## 11. Холбоо барих

{{Блүпринт Солюшнс ХХК}} · {{хаяг}} · {{имэйл}} · {{утас}}

---

# Privacy Policy — Blueprint Merchant (English)

> The Mongolian version above prevails in case of any difference.

**Effective date:** {{YYYY-MM-DD}}

## 1. Who we are

Blueprint Merchant is developed and operated by {{Blueprint Solutions LLC, full legal name}} ("Blueprint", "we"), {{address}}, {{email}}, {{phone}}. The app lets staff of a shop or business order from the suppliers that have registered their business as a customer. Staff use the app on behalf of their employer. We process personal data under the Law of Mongolia on Personal Data Protection and other applicable law.

## 2. Data we collect

- **Sign-in (BP ID):** you sign in with a BP ID account. Your password is entered on BP ID's page; the app never sees or stores it. BP ID passes us your name, phone number, email address and account identifier.
- **Business and branch:** your employer's name and registration number, and the names, addresses and phone numbers of the branches you are assigned to, as set up by your employer's administrator.
- **Orders:** products and quantities in your cart, orders you send, requested delivery dates, notes, and order and delivery status.
- **Technical data:** server logs needed to run the service, such as request IDs and timestamps.

**We do not collect** location, contacts, photos, camera or microphone data, payment card data or advertising identifiers. The app shows no ads and does not track you across other apps or websites.

## 3. How we use it

To sign you in and identify your business and branch; to show your suppliers' contract products and prices; to deliver your orders to suppliers and show their progress; and to fix errors and keep the service secure. We do not sell your data or use it for advertising.

## 4. Who we share it with

- **Suppliers** receive the orders you send them: the order lines, the delivery branch's name, address and phone, the requested date and your note. They do not see your business's other branches.
- **Your employer's** authorised staff can see orders placed on its behalf.
- **Service providers** acting on our instructions, such as hosting ({{provider, country}}).
- **Authorities**, where required by law.

## 5. Data stored on your device

Sign-in tokens are kept in the device's secure storage (iOS Keychain, Android Keystore). Your cart, selected branch and a cache of product details (names, codes, barcodes; not prices or stock) are kept so the app works quickly and offline. This data is kept separately for each account and business. **Signing out** (Бүртгэл → Гарах) deletes all of it from the device, as does uninstalling the app.

## 6. Retention

Orders are kept for {{period, e.g. as required by accounting law}}. Server logs are kept for {{period}}. BP ID account data is governed by BP ID's privacy policy: {{link}}.

## 7. Security

All traffic between the app and our servers is encrypted (HTTPS). Sign-in tokens are kept in secure storage. The server checks your business and branch on every request, so you cannot access another business's or branch's data.

## 8. Your rights

You may request access to, correction or deletion of your personal data, or object to its processing, by writing to {{email}}. We will respond within {{number}} days. Your name, phone, business and branch details are managed by your employer's administrator, so please ask them first for corrections. Suppliers may keep orders they received as required by law.

**Account deletion:** {{how to request it — email or web page; required by Google Play and the App Store}}.

## 9. Children

The app is meant for business staff and is not directed at anyone under 18.

## 10. Changes

We will post any update here and change the effective date. We will tell you in the app about significant changes.

## 11. Contact

{{Blueprint Solutions LLC}} · {{address}} · {{email}} · {{phone}}
