# AnkiAudio

Proste narzędzie do generowania fiszek z plikami audio dla AnkiDroid.

---

## Wymagania

1. [Termux w Google Play](https://play.google.com/store/apps/details?id=com.termux)
2. [Termux:API w Google Play](https://play.google.com/store/apps/details?id=com.termux.api)

Zakładamy, że masz obie aplikacje zainstalowane.

---

## Instalacja w Termuxie

Skopiuj i wklej w Termuksie:

```sh
# Aktualizacja i podstawowe narzędzia
pkg update
pkg install python pipx git termux-api -y

# Instalacja gTTS
pipx install gtts

# Utworzenie katalogu ~/bin jeśli nie istnieje
mkdir -p ~/bin

# Ściągnięcie skryptu ankiaudio
cd ~/bin
curl -LO https://raw.githubusercontent.com/Kismetus/ankiaudio/main/ankiaudio.py

# Nadanie praw do uruchamiania
chmod +x ankiaudio.py
