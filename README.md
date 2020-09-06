# quran-log

[The plan]

Need to set constants.
- what rasm to use. (strong suggestion, rasm Uthmani, read page by page)
- language UI (definately Bahasa Melayu as Primary. English is not in current plan)
- the homepage UI & UIX (whats on it, without clutter, and easy to use)
- planning & development team/person (aizu.)
- test user (aizu.)

## Objective
- Primary objective: To increase motivation to read Quran, bit by bit, by seeing the progress made throughout the journey.
- Visually see the progress.
- Keep track, what we've read last. Not many of us, stick with specific Quran to read. Some of us, read on printed copy, same copy all the time. Some of us, read on phone.

## Process
- Link to quran.com / alquran.my to specific surah that going to read.
- Manually mark, which verse already read.
- Marking are set to each verse.

### User Interface
- Bahasa Melayu (primary language)
- Progress bar overall (114 Surahs)
- List by Pages (Rasm Uthmani / alquran.my) - 604 pages
- List of Surah.
- List of Verse, by dot or line.
- Calander view, can see my own reading Quran habit.

### Technology
- Web app, via browser & URL.
- Save progress in server, key in browser's cookies.
  - Offer to have reference to the key by Google Login
  - Absolutely basic auth, probably just email & hash
  - Passport
- Open source. Credentials & secrets will be in .env
- NextJS, hosted in aizu.my
  - Subdomain: quranlog.aizu.my / quran-log.aizu.my
  - PM2 ecosystem, commit.sh
  - Multiple components, multiple pages
  - Need to plan, the pages, and whats on the page
  
### Pages
- Homepage
  - Show main Quran progress (6,236 verses)
    - Progress bar horizontal
  - List of surahs, 114 items
    - List by pages (Rasm Uthmani)
      - interaction: tick (multiple icons)
        - Recite (Bacaan sahaja)
        - Recite & meaning (Bacaan & maksud)
        - Meaning (Maksud sahaja)
      
- Calendar
  - https://projects.wojtekmaj.pl/react-calendar/ ?
- Login / Account
  - If Guest user, show sign up form
  - If Logged user, show basic details & logout

### Notes
- Need to teach user, where the appropreate verse to stop read & continue next session.

## Figures
- 114 Surah
- 6,236 Verses
- 30 Juz
- 604 pages on rsam Uthmani
- Most verses in quran: Surah Al-Baqarah, 286 verses
  - Surah As-Shura (227 verses)
  - Surah Al-Araf (207 verses)
  - Surah Al-Imran (200 verse)
 
## Others
Q: So Aizu, are you going to use it ?
A: Yes. Me myself, personally I'll use it. Why? My motivation to finish up the whole book. I've been reading Quran from the printed, a various format. Sometimes, the quran.com or downloaded mobile app is more convinience. I always lost, where the last verse that I stopped. Primitive way, I jot down in Telegram Saved message.

Ref;
- https://www.quora.com/What-are-the-seven-longest-surahs-in-the-Holy-Quran
