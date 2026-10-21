# Product

<!-- impeccable:product-schema 1 -->

## Platform

android

Android **tablet**, landscape. Every screen in the Figma design is 1280×800, and the copy says videos are "Tersimpan di tablet". Phone layouts are not designed.

## Stack

Kotlin + Jetpack Compose (native Android).

## Users

Elderly people (lansia), who use the app themselves on a tablet. Each person has their own account (for example "siti01, Ibu Siti"). The app addresses them politely by name and honorific ("Halo, Ibu Siti!").

Who hands out the tablets and creates the accounts (a study team, posyandu, caregivers or a care facility) is not yet recorded.

## Product Purpose

A 6-week program that helps elderly users keep their brain active. Each week the user:

1. Completes the **IADL** questionnaire about everyday activities.
2. Takes the **RUDAS** memory and thinking test.
3. Does the **Aktivitas** exercises.

Progress is saved to the user's account and shown week by week.

What success means beyond completing the 6 weeks (for example adherence, changes in RUDAS scores, or who reads the results) is still open.

## Positioning

Still open. The design shows a structured weekly program that pairs two established elderly assessments (IADL and RUDAS) with guided physical and cognitive activities, instead of open-ended brain games. No competitive claim has been confirmed.

## Operating Context

These are the screens and sections in the Figma file "Sehat Lansia — Desain v3":

- **Masuk (login):** username and password ("Selamat Datang", "Silakan masuk ke akun Anda").
- **Menu utama (home):** three cards.
  - IADL shows the weekly progress, for example "Minggu ke-3 selesai, 3/6".
  - RUDAS shows the best score, for example "24/30".
  - AKTIVITAS shows the points collected, for example "120 Poin terkumpul".
  - Also on the screen: Pengaturan (settings) and Keluar (exit). Exiting asks for confirmation ("Keluar dari aplikasi?") and reassures the user that their progress is saved.
- **IADL (Kuesioner kegiatan harian):**
  - A week strip for Minggu 1–6 with the states Selesai (done), Minggu ini / Belum diisi (this week, not filled in) and Nanti (locked until later).
  - An info screen: "Kuesioner ini menanyakan kegiatan sehari-hari, seperti memasak, berbelanja, dan minum obat. Diisi satu kali setiap minggu, sebelum senam."
  - Single-choice questions, then a thank-you screen when it's complete.
- **RUDAS (Tes daya ingat):**
  - The same week strip, showing each week's score out of 30 and whether it went up ("Naik").
  - 6 short questions. One of them asks the user to copy a cube drawing with their finger ("Gambar di sini dengan jari").
  - A results screen with this week's score and the change from last week.
- **Aktivitas:**
  - **Senam:** a 30-minute elderly exercise video. The weekly IADL must be filled in first. If it isn't, a reminder appears with "Isi sekarang" and "Nanti saja".
  - **Brain Gym:** a 45-minute guided-movement video, followed by questions about the movements. +10 points for each correct answer.
  - **Music Games:** a short random video, then the user guesses the sound or picture. The answer choices are Indonesian instruments (angklung, gamelan, suling, kendang). +10 points for each correct answer.
  - **Hasil poin (points result):** the points from each question, the total, and encouraging copy ("Hebat! Jawaban benar 3 dari 3.").
- **Pengaturan (settings):**
  - Text size (A−/A+, default 32).
  - Language for text and voice: Indonesia or English.
  - Voice guide on or off, which reads questions and information aloud.
  - The account the progress is saved to.

## Capabilities and Constraints

- **Program structure:** 6 weeks. Past weeks are complete, the current week is open, and future weeks are locked.
- **Weekly order:** IADL must be filled in before Senam each week.
- **Points:** earned in Brain Gym and Music Games, +10 for each correct answer, and saved to the account.
- **Accounts:** each user signs in with a username and password, and progress is tied to the account.
- **Languages:** Bahasa Indonesia is the default; English is also offered. Both apply to text and to voice.
- **Text-to-speech or recorded voice:** the app reads questions and information aloud.
- **Exercise videos:** stored on the tablet, so playback works without internet. Whether the rest of the app works offline is still open.
- **Not in the product:** health or vitals tracking, and free-form brain games such as memory cards or puzzles.
- **Still open:**
  - Where accounts and progress are stored (backend or on the device).
  - Who creates accounts.
  - The exact IADL and RUDAS item wording, the scoring rules, and their sources.
  - The full Brain Gym and Music Games question banks.
  - Whether results are shared with anyone else.

## Brand Commitments

- **Name:** the design file is named "Sehat Lansia"; the repository is named AplikasiLansia. Which one is the app's public name is still open.
- **Voice:** warm, polite and encouraging Indonesian. The user is addressed as Ibu or Bapak by name, and sentences are short ("Isi kuesioner IADL dulu, ya", "Hanya sekitar 5 menit").
- **Visual authority:** the Figma file "Sehat Lansia — Desain v3" (https://www.figma.com/design/O5ppdNOoiwLWhEovqGpQFv) is the approved design. Its visual system will be recorded in DESIGN.md separately.

## Evidence on Hand

- The Figma design, with 18 screens (01–19; there is no 05).
- No real question banks, exercise videos, instrument photos or audio are in the repository yet. The design uses placeholders such as "[Foto angklung]" and "Contoh video". Future work must not invent clinical results, endorsements or claims about health outcomes.

## Product Principles

1. **One clear weekly path.** The user always knows what this week asks of them and what comes next. Locked future weeks and the IADL-before-Senam order keep the program simple.
2. **Encourage, never judge.** Scores and points are shown as progress ("Naik 1 poin", "Hebat!"). Assessment results are never framed as failure, decline or diagnosis.
3. **Assessments stay faithful.** IADL and RUDAS are standard instruments, so the app keeps their wording and scoring intact and doesn't gamify them. Points belong only to Aktivitas.
4. **Usable alone.** Every screen works for an older adult using the tablet without help: read aloud, adjustable text size, and progress that is always saved.
5. **Familiar and local.** Indonesian language, honorifics and cultural content (traditional instruments, senam lansia) come first.

## Accessibility & Inclusion

The design itself commits to these:

- Text size the user can adjust, with a large default.
- A voice guide that reads questions and information aloud.
- Large touch targets and buttons with text labels.
- Every user action gets clear feedback.
- The drawing task uses a finger, not a stylus.

These are inferred from the elderly audience; no formal standard has been chosen:

- High contrast.
- No time pressure on any answer.
- No reliance on fine motor gestures beyond the drawing task.
