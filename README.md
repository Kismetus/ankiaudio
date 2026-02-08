# Ankiaudio

Prosty skrypt do generowania fiszek z plikami audio dla AnkiDroid w Termuxie.

---

## 1. Wymagania

1. [Termux](https://play.google.com/store/apps/details?id=com.termux)  
2. [Termux:API](https://play.google.com/store/apps/details?id=com.termux.api)

Po zainstalowaniu obu aplikacji zakładamy, że są gotowe do użycia.

---

## 2. Instalacja zależności i skryptu

Skopiuj i wklej do Termuxa (całość na raz):

```sh
# aktualizacja pakietów
pkg update && pkg upgrade -y

# instalacja Python i pipx
pkg install python pipx -y

# instalacja gTTS
pipx install gtts

# utworzenie katalogu na skrypty
mkdir -p ~/bin

# pobranie skryptu ankiaudio
curl -o ~/bin/anki-audio https://raw.githubusercontent.com/Kismetus/ankiaudio/main/ankiaudio.py

# nadanie praw do uruchamiania
chmod +x ~/bin/anki-audio

# gotowe, od teraz można uruchamiać skrypt z dowolnego miejsca:
# anki-audio
