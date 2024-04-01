# Responding to Reviewer Comments - LaTeX Template

This LaTeX template provides a convenient format for responding to reviewer comments for the journal "Smart Factory & Energy Efficiency." It includes features such as setting the journal title, journal logo, editor's name, date, reviewer comments, responses, and the author's name.

## Getting Started

To use this template for responding to reviewer comments, follow these steps:

1. **Clone the Repository**: Clone this repository to your local machine.

2. **Configure the Template**: Open the `letter_sfee.sty` file and configure the following parameters:
   - `journalTitle`: Set the title of the journal to "Smart Factory & Energy Efficiency."
   - `journalLogo`: Set the path to the journal logo file.
   - `editorName`: Set the name of the editor handling the review process.
   - Optionally, adjust other parameters such as font sizes, colors, etc.

3. **Create Your Response Letter**: In your LaTeX document (e.g., `response_letter.tex`), include the `letter_sfee` package and set the required parameters:
   - `\journalTitle`: Set the title of the journal to "Smart Factory & Energy Efficiency."
   - `\journalLogo`: Set the path to the journal logo file.
   - `\editorName`: Set the name of the editor handling the review process.
   - `\letterDate`: Set the date of your response letter.
   - Optionally, include the author's name using `\authorName`.

4. **Write Your Response**: Write your responses to the reviewer comments in the body of the letter, using the provided format for reviewer comments and responses.

5. **Compile the Document**: Compile your LaTeX document using your preferred LaTeX compiler (e.g., `pdflatex`).

6. **View Your Response Letter**: Open the compiled PDF file to view your response letter.

## Example

```latex
\documentclass{letter}
\usepackage{letter_sfee}

% Package configuration
\journalTitle{Smart Factory & Energy Efficiency}
\journalLogo{logo_sfee.png}
\letterDate{31}{03}{2024}
\authorName{John Doe}
\editorName{Juan de Anda Suárez}

\begin{document}

\begin{letter}{Recipient}
\opening{}

This is the body of the response letter.

\begin{reviewer}{}
\comment{Reviewer 1 comment}
\response{Response to reviewer 1 comment}

\comment{Another comment from reviewer 1}
\response{Response to another comment from reviewer 1}
\end{reviewer}

\begin{reviewer}{}
\comment{Reviewer 2 comment}
\response{Response to reviewer 2 comment}
\end{reviewer}

\closing{Sincerely, \authorName}
\end{letter}

\end{document}

