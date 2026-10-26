# Health Diary

Личный трекер питания, шагов, тренировок, веса и замеров.

Frontend: static GitHub Pages website (`index.html`). Backend: Supabase Auth and PostgreSQL with row-level security.

## Публикация

GitHub → Settings → Pages → Build and deployment → Deploy from a branch → main → / (root) → Save.

## Авторизация

Supabase project `eqfklqcbemutyninqcid` → Authentication → URL Configuration. Add `https://komissarSaroka.github.io/health-diary/` as Site URL and Redirect URL. Настройка SMTP и лимитов отправки писем зависит от Supabase Auth.

## Данные

Хранятся в `public.diary_entries`; пользователи имеют доступ только к своим строкам благодаря RLS. В интерфейсе доступен экспорт и импорт JSON.
