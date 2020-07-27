RETAS OCR EVALUATION DATASET

Purpose and Characteristics:
----------------------------
This dataset is created to evaluate optical character recognition (OCR) accuracy of scanned books. It consists of:
-	OCR output of 160 scanned books (100 English, 20 French, 20 German, 20 Spanish) downloaded from the Internet Archives website (www.archive.org)
-	Corresponding ground truth text for each book. They are obtained from the Project Gutenberg website (www.gutenberg.org)
-	Word and char level alignment outputs. Each OCR output is aligned with the ground truth text using REcursive Text Alignment Scheme (RETAS).
-	Estimated OCR accuracies. 
For the purposes of OCR evaluation, any extra material (e.g. Project Gutenberg and Internet Archives disclaimers) in the front or rear is removed so that the books are as close to the ground truth as possible.

Citation Information:
---------------------
If you make use of RETAS dataset, please use the following citation:
I. Zeki Yalniz and R. Manmatha, A Fast Alignment Scheme for Automatic OCR Evaluation of Books. To appear in the Proceedings of ICDAR'11.

Dataset Information:
--------------------
-> Data is contained in three folders:
1. \IA_texts includes OCR outputs of all scanned books, categorized by language (UTF-8).
2. \GUT_texts includes the ground truth texts of scanned books, categorized by language (UTF-8).
3. \alignment_outputs includes the alignment outputs, categorized by language (UTF-8).

-> Lists of filename pairs <OCR OUTPUT, GROUND TRUTH> is also included for each scanned book in the dataset. They are categorized by language.
eng_pairs.txt
fre_pairs.txt
ger_pairs.txt
spa_pairs.txt

-> Estimated OCR accuracies are included in OCR_accuracy_list.xls file.

Format of the Alignment Output:
-------------------------------
There are four alignment outputs for each book pair. Namely,

<OCRfilename>-<GTfilename>.wcol: word level alignment output in the two-column format.
<OCRfilename>-<GTfilename>.wline: word level alignment output in the line format. 
<OCRfilename>-<GTfilename>.ccol: char level alignment output in the two-column format. 
<OCRfilename>-<GTfilename>.cline: char level alignment output in the line format. 

In the line format, each line contains 20 words. OCR output and the ground truth lines are indicated by "OCR:" and "GT :" tags respectively. Line format is more convenient  for manual inspection of the alignment output. 
In the two-column format, the OCR output is the first column. Words/characters which does not align with any word/character on the other sequence are aligned with empty string. In the alignment output, empty string and characters are indicated by "null" and "@" respectively. 


IMPORTANT NOTICE:
-----------------
According to the Project Gutenberg and Internet Archive websites, the books are out of copyright in the United States. This may not be the situation in a particular country so you are advised to check this and follow the law of your country. If you just want to read the book you are better off looking at their websites where they have much nicer interfaces for doing this. Note that the Internet Archives website may update their files at any time. In this case we do not know the specifics of the OCR and preprocessing they use. 

THIS DATA IS PROVIDED BY UNIVERSITY OF MASSACHUSETTS AND OTHER CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDERS OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS DATA, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

For further questions, please contact I. Zeki Yalniz (zeki[at]cs[dot]umass[dot]edu)
