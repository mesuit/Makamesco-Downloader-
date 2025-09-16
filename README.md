# LEONARD-MD

![LEONARD Typing Banner](assets/typing.svg)

**Leo ni leo — tuma, jaribu, andika!**

## Maelezo
LEONARD-MD ni bot ya WhatsApp/pair code inayoruhusu watumiaji kuunganisha session kupitia link ya Session ID. Mradi huu unaambatanisha huduma ya session yako ya demo ili watu waweze kujaribu kwa haraka.

👉 Demo/Session: https://leonard-session-091.onrender.com

## Sifa kuu
- Rahisi ku-fork na ku-deploy
- Mwonekano wa jina (typing SVG) kwa header ya README
- Maelekezo ya haraka ya deploy (Heroku / Render / Docker)

## Jinsi ya kuanza (Quickstart)
1. Fork repo hii: `https://github.com/leonard1tech/LEONARD-MD`
2. Unda folda `assets/` kisha weka `typing.svg` ndani yake (angalia `assets/typing.svg` mfano chini).
3. Hariri `config` au `.env` kuweka `SESSION_ID` au endpoints zako.
4. Deploy kwa Heroku / Render / Vercel au kutumia Docker.

## Deploy kwa Heroku (kwa haraka)
1. Login Heroku CLI: `heroku login`
2. Create app: `heroku create your-app-name`
3. Add repo remote: `git push heroku main`
4. Set environment vars:  
   `heroku config:set SESSION_ID=your_session_value`
5. Open app: `heroku open`

> Ikiwa unahitaji timu za Heroku au msaada wa hatua za mwisho, tuma ujumbe nami nikusaidie.

## Kujaribu locally (Docker)
```bash
docker build -t leonard-md .
docker run -e SESSION_ID="your_session" -p 3000:3000 leonard-md
