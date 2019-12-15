# ADoNoSnips
... try to replace all Snips technology from the Snips-based assistent ...

Snips.AI announced in Dec 2019 that it will go commercial and some of the main components will no longer
be available to the public.
This repo tries to replace all Snips-technology by other systems (homegrown, if possible) step-by-step.
These are

- Hotword detection (easy job: Snowboy is on-device too and even better)
- ASR (not so easy; in a first attempt, Google STT will be implemted; 
  however on-device STT ist the goal!)
- NLU (even more simple: Snips style, to have skill-code at GitHub and the rules for skill recognition
  in the Snips console have been annoying since the beginnen.
  Goal is to integrate NLU in the Skill code)
- logs and watch-service.
  
The idea behind the project is, to build new services that publish and subscribe to Snips-compatible
MQTT messages, so that exsisting (and future) Snips skills keep beeing interoperable with the framework.
