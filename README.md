# ftm-languagepacks
Language packs for Feed the Monster localizations

# Usage
Used with the Feed the Monster Core, which contains all language-independent data for Feed the Monster, found here: https://github.com/curiouslearning/FeedTheMonster/tree/newCore

# Creating a New Language Pack
Use the FTMdefault directory as a template for your language pack directory. Configure the settings.json file as needed, and replace the image and sound assets from the subfolders with the appropriate images and sound assets for your language.

## settings.json
The settings.json file is used to define settings for the language, as follows:
field | usage
------ | ------
"LanguageName" (string) | the name of the language
"ApplicationName" (string) | the name of the game, i.e. "Feed the Monster", in the language
"VersionNumber" (int) | the Android version number of the game
"ImageBasedRendering" (bool) | whether the language uses images of each character instead of Unity's default text rendering
"NumLevels" (int) | the number of levels in the game, usually 77 or 154
"HasTracingGame" (bool) | whether to include the letter-tracing game, which is based on the latin alphabet characters

## Language Pack Structure
subfolder | contents
--------- | --------
/charimg | contains the character images, if a image-based rendering system is used
/levels | contains the level xml files
/sounds/letters | contains audio files for each character taught in the game
/sounds/words | contains audio files for each word taught in the game
/sounds/feedbacks | contains positive feedback audio
/sounds/other | contains instruction audio
/art/feedbacks | contains gold positive feedback text images
/art/titles |  contains blue ui text images
/art/memg | contains the icon, word, and audio assets for the memory game

## Filenames

### sounds/letters
The audio files in this folder should be named according to how characters are referenced in the level xml files, i.e. 'a.wav' or '1.wav'

### sounds/letters
The audio files in this folder should be named according to how words are referenced in the level xml files, i.e. 'cat.wav'

### sounds/feedbacks
The asset files in this folder must have the following names:
* amazing work.wav
* fantastic work.wav
* fantastic1.wav
* great1.wav

### sounds/other
The asset files in this folder must have the following names:
* are_you_sure.wav
* bonus_treasure.wav
* im_angry.wav
* im_bored.wav
* im_sad.wav
* lets_write_letters.wav
* new_friend.wav
* pet_me.wav
* playing_together.wav
* select_monster.wav
* select_player.wav
* thanks_better.wav
* thanks_happy.wav
* try_letter.wav
* watch_grow.wav

### /art/feedbacks
The asset files in this folder must have the following names:
* 2_txt_fantastic_glow.png
* 2_txt_fantastic_shimmer_sheet.png
* 3_txt_fantastic_work_glow.png
* 4_txt_great_glow.png
* 4_txt_great_shimmer_sheet.png
* Amazing_Work_01.png
* amazing_work_glow.png
* amazing_work_shimmer_sheet.png
* Fantastic_01.png
* FantasticWork_01.png
* fantastic_work_shimmer_sheet.png
* Great_01.png


### /art/titles
The asset files in this folder must have the following names:
* are_you_sure.png
* lets_write_some_letters.png
* parents_progression_LETERS.png
* parents_progression_VOWELS.png
* parents_progression_WORDS.png
* pet_me.png
* SEL_popup_AngryText_v01.png
* SEL_popup_BoredText_v01.png
* SEL_popup_SadText_v01.png
* select_your_player.png
* Selection_choose_your_monster 01.png
* Splash_screen_v03_logo.png
* Treasure_feedback_01.png

### /art/memg
The memory game word assets come in sets of three memg_x_x_a.jpg (an image of the text of the word), memg_x_x_b.jpg (a picture of what the word represents), and memg_x_x_c.wav (the pronunciation of the word).

The asset files in this folder must have the following names:
* memg_2_1_a.jpg
* memg_2_1_b.jpg
* memg_2_1_c.WAV
* memg_2_2_a.jpg
* memg_2_2_b.jpg
* memg_2_2_c.wav
* memg_2_3_a.jpg
* memg_2_3_b.jpg
* memg_2_3_c.wav
* memg_2_4_a.jpg
* memg_2_4_b.jpg
* memg_2_4_c.wav
* memg_2_5_a.jpg
* memg_2_5_b.jpg
* memg_2_5_c.WAV
* memg_2_6_a.jpg
* memg_2_6_b.jpg
* memg_2_6_c.wav
* memg_3_1_a.jpg
* memg_3_1_b.jpg
* memg_3_1_c.WAV
* memg_3_2_a.jpg
* memg_3_2_b.jpg
* memg_3_2_c.WAV
* memg_3_3_a.jpg
* memg_3_3_b.jpg
* memg_3_3_c.wav
* memg_3_4_a.jpg
* memg_3_4_b.jpg
* memg_3_4_c.WAV
* memg_3_5_a.jpg
* memg_3_5_b.jpg
* memg_3_5_c.wav
* memg_3_6_a.jpg
* memg_3_6_b.jpg
* memg_3_6_c.WAV
* memg_4_2_a.jpg
* memg_4_2_b.jpg
* memg_4_2_c.WAV
* memg_4_3_a.jpg
* memg_4_3_b.jpg
* memg_4_3_c.WAV
* memg_4_4_a.jpg
* memg_4_4_b.jpg
* memg_4_4_c.wav
* memg_4_5_a.jpg
* memg_4_5_b.jpg
* memg_4_5_c.WAV
* memg_5_1_a.jpg
* memg_5_1_b.jpg
* memg_5_1_c.WAV
* memg_5_2_a.jpg
* memg_5_2_b.jpg
* memg_5_2_c.WAV
* memg_5_3_a.jpg
* memg_5_3_b.jpg
* memg_5_3_c.wav
* memg_5_5_a.jpg
* memg_5_5_b.jpg
* memg_5_5_c.WAV
* memg_5_6_a.jpg
* memg_5_6_b.jpg
* memg_5_6_c.WAV
* memg_6_1_a.jpg
* memg_6_1_b.jpg
* memg_6_1_c.wav
