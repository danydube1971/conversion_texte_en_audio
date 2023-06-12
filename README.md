# conversion_texte_en_audio
Permet de convertir un fichier txt en audio WAV par synthèse vocale de Google
Ce script utilise la bibliothèque gTTS (Google Text-to-Speech) pour convertir un fichier texte en un fichier audio au format WAV en français. Voici ce que fait chaque partie du script :

La ligne from gtts import gTTS importe la classe gTTS de la bibliothèque gTTS, qui est responsable de la conversion du texte en audio.

La fonction convert_text_to_speech(text, output_file) prend en entrée le texte à convertir et le nom du fichier de sortie, puis effectue les opérations suivantes :

Elle utilise gTTS(text, lang='fr') pour créer un objet gTTS en spécifiant la langue française (lang='fr').
Ensuite, elle utilise la méthode save(output_file) pour enregistrer l'audio généré dans un fichier WAV.
Les variables input_file et output_file sont définies pour représenter respectivement le chemin vers le fichier texte d'entrée et le chemin vers le fichier audio de sortie.

Le contenu du fichier texte est lu en utilisant open(input_file, 'r', encoding='utf-8') as file et est stocké dans la variable text.

La fonction convert_text_to_speech(text, output_file) est appelée avec les arguments text et output_file pour effectuer la conversion du texte en audio et enregistrer le fichier audio.

Enfin, le message 'Conversion terminée !' est affiché pour indiquer que la conversion a été effectuée avec succès.

En résumé, ce script prend un fichier texte en français, utilise la bibliothèque gTTS pour le convertir en audio, puis enregistre le fichier audio résultant au format WAV.
