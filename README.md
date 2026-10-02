# Jorge Laban

**Full-Stack Developer** · Lima, Peru

I build web and mobile apps end to end: the data model, the backend and the screen people actually use.

Open to remote and on-site full-stack roles starting December 2026.

**Languages:** Spanish (native) · English (advanced, C1) · Portuguese (basic)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jorge-laban-hijar)

## Tech stack

<p>
  <img src="https://skillicons.dev/icons?i=java,spring,ts,js,react,angular,nodejs,flutter,dart,postgres,mysql,supabase,docker,aws,azure,cloudflare,git&perline=17" alt="Java, Spring Boot, TypeScript, JavaScript, React, Angular, Node.js, Flutter, Dart, PostgreSQL, MySQL, Supabase, Docker, AWS, Azure, Cloudflare, Git" />
</p>

**Backend:** Java (Spring Boot) · Node.js (Express) · REST APIs · SQL (PostgreSQL, MySQL, SQLite) · Supabase

**Frontend & mobile:** JavaScript / TypeScript · React · Angular · Flutter (Dart)

**Cloud & tools:** Docker · AWS · Azure · Cloudflare · Git / GitHub

**Also:** Python · PHP and Laravel (basic)

## Featured projects

### Tienda con microservicios — Spring Boot and Spring Cloud

A store split into five services that shows four distributed-systems patterns with scenarios you can reproduce.

- **Saga** orchestrated by the orders service: reserve stock, then charge; if a step fails, compensations release the stock or refund the payment, and they are retried until they complete.
- **Circuit Breaker** (Resilience4j) on the calls to inventory and payments, **API Gateway** that only publishes read endpoints, and **Config Server** with the configuration of every service.
- One PostgreSQL database per service, 43 tests (JUnit 5, Mockito) and GitHub Actions that runs them and builds the Docker images.

`Java 21` `Spring Boot 3.5` `Spring Cloud` `Resilience4j` `PostgreSQL` `Docker`

[Code](https://github.com/jarlh19/tienda-microservicios)

### Mi Plato — from a meal photo to nutrition facts

<img src="https://raw.githubusercontent.com/jarlh19/mi-plato/main/docs/screenshots/diary.png" width="160" alt="Mi Plato daily summary"> <img src="https://raw.githubusercontent.com/jarlh19/mi-plato/main/docs/screenshots/verdict.png" width="160" alt="Mi Plato meal verdict">

Take a photo of your plate and get calories, macros and a verdict on the meal.

- A vision model only identifies the foods and estimates their weight; the nutrients come from USDA FoodData Central.
- The verdict (BMI, daily target, pros and cons) is plain Dart with fixed rules based on WHO thresholds, so the same plate always gets the same answer. It is covered by unit tests.
- Daily analysis quota enforced in Postgres, plus account deletion and data export.
- Runs in demo mode without a backend.

`Flutter` `Supabase` `Edge Functions` `PostgreSQL`

[Code](https://github.com/jarlh19/mi-plato)

### Tienda de Barrio — an app for a neighborhood store

<img src="https://raw.githubusercontent.com/jarlh19/tienda-barrio/main/docs/screenshots/catalog.png" width="160" alt="Tienda de Barrio catalog"> <img src="https://raw.githubusercontent.com/jarlh19/tienda-barrio/main/docs/screenshots/production-recipe.png" width="160" alt="Tienda de Barrio production costed from the recipe">

Customers browse the catalog, fill a cart and place orders; the shopkeeper runs the store from their own panel.

- Stock intake by scanning barcodes: a known code opens the product to restock it, a new one opens the form already filled in.
- A single inventory ledger drives both stock and cash. Ingredients are costed by weighted average and each product has an editable recipe, so it also works for a bakery.
- Payments through Yape and Plin (Peruvian mobile wallets) verified by operation number, plus store credit for regular customers.
- Key decisions recorded as ADRs. Runs in demo mode without a backend.

`Flutter` `Supabase` `PostgreSQL`

[Code](https://github.com/jarlh19/tienda-barrio)

### Flores Amarillas — a personalized 3D flower garden

<img src="https://raw.githubusercontent.com/jarlh19/flores-amarillas/main/docs/screenshots/editor.jpg" width="480" alt="Flores Amarillas editor with live 3D preview">

A web app to build a 3D sunflower garden as a gift, with your own photos and messages.

- Editor with live preview that creates a shareable link or a standalone HTML file.
- Gifts are stored in Cloudflare D1 through Pages Functions. Photos are resized in the browser and creation is rate-limited per hashed IP.
- Music plays through the YouTube IFrame API, so no audio is hosted.

`JavaScript` `three.js` `Cloudflare Pages` `D1`

[Live demo](https://regala-flores-amarillas.pages.dev) · [Code](https://github.com/jarlh19/flores-amarillas)
