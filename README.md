# resume

\documentclass[letterpaper,10pt]{article}

\usepackage{makecell}
\usepackage[link=off]{phonenumbers}

\usepackage{latexsym}
\usepackage[empty]{fullpage}
\usepackage{titlesec}
\usepackage{marvosym}
\usepackage[usenames,dvipsnames]{color}
\usepackage{verbatim}
\usepackage{enumitem}
\usepackage[pdftex]{hyperref}
\usepackage{fancyhdr}


\pagestyle{fancy}
\fancyhf{} % clear all header and footer fields
\fancyfoot{}
\renewcommand{\headrulewidth}{0pt}
\renewcommand{\footrulewidth}{0pt}
\usepackage[margin=0.3in]{geometry}
% Adjust margins
\addtolength{\oddsidemargin}{-0.0in}
\addtolength{\evensidemargin}{-0.0in}
\addtolength{\textwidth}{0in}
\addtolength{\topmargin}{20pt}
\addtolength{\textheight}{0.0in}

\urlstyle{same}

\usepackage{xcolor}% http://ctan.org/pkg/xcolor
\usepackage{hyperref}% http://ctan.org/pkg/hyperref
\hypersetup{
  colorlinks=true,
  linkcolor=blue!50!red,
  linkbordercolor=red,
  urlcolor=blue!70!black
}

\raggedbottom
\raggedright
\setlength{\tabcolsep}{0in}

% Sections formatting
\titleformat{\section}{
  \vspace{-10pt}\scshape\raggedright\large
}{}{0em}{}[\color{black}\titlerule \vspace{-7pt}]

%-------------------------
% Custom commands
\def \ifempty#1{\def\temp{#1} \ifx\temp\empty }

\newcommand{\resumeItem}[2]{
  \item\small{
  	\ifempty{#1}#2\else\textbf{#1}{: #2 \vspace{-2pt}}\fi
  }
}

\usepackage[dvipsnames]{xcolor}
\definecolor{mygray}{gray}{0}
\usepackage{fancybox}

\usepackage{lmodern}
\usepackage{tikz}

% Style definition
\tikzset{rndblock/.style={rounded corners,rectangle,draw,outer sep=0pt}}

% Command Definition
% 1 optional to customize the aspect, 2 mandatory: text to be framed
\newcommand{\tframed}[2][]{\tikz[baseline=(h.base)]\node[rndblock,#1] (h) {\color{black}{#2}};}

\newcommand*{\mystrut}{\rule[-0.2\baselineskip]{0pt}{0.8\baselineskip}}
\newcommand{\skill}[1]{\tframed[lightgray]{\mystrut#1}}


\newcommand{\resumeSubheading}[4]{
  \vspace{-1pt}\item
    \begin{tabular*}{0.97\textwidth}{l@{\extracolsep{\fill}}r}
      \textbf{#1} & \textcolor{mygray}{#2} \\
      \textit{\small#3} & \textcolor{mygray}{\textit{\small #4}} \\
    \end{tabular*}\vspace{-5pt}
}

\newcommand{\resumeExpSubheading}[5]{
  \vspace{-1pt}\item
    \begin{tabular*}{0.97\textwidth}{l@{\extracolsep{\fill}}r}
      \textbf{#1}  & \textcolor{mygray}{#2} \\
      \textit{\small#3} & \textcolor{mygray}{\textit{\small #4}} \\
      {\scriptsize#5}
    \end{tabular*}\vspace{4pt}
}

\newcommand{\resumeProjSubheading}[4]{
  \vspace{-1pt}\item
    \begin{tabular*}{0.97\textwidth}{l@{\extracolsep{\fill}}r}
      \textbf{#1}  & \textcolor{mygray}{#2} \\
      \scriptsize {#3} & \textcolor{mygray}{\textit{\small #4}} \\
    \end{tabular*}\vspace{4pt}
}

\newcommand{\resumeSubItem}[2]{\resumeItem{#1}{#2}\vspace{-4pt}}

\renewcommand{\labelitemii}{$\circ$}

\newcommand{\resumeSubHeadingListStart}{\begin{itemize}[leftmargin=*]}
\newcommand{\resumeSubHeadingListEnd}{\end{itemize}}
\newcommand{\resumeItemListStart}{\begin{itemize}[leftmargin=0.2in]}
\newcommand{\resumeItemListEnd}{\end{itemize}\vspace{-5pt}}

\usepackage{changepage}
\newcommand{\resumeDesc}[1]{\begin{adjustwidth}{5pt}{0pt}\vspace{-2pt}{\small{#1}}\end{adjustwidth}}

%-------------------------------------------
%%%%%%  CV STARTS HERE  %%%%%%%%%%%%%%%%%%%%%%%%%%%%


\begin{document}

%----------HEADING-----------------
\begin{tabular*}{\textwidth}{l@{\extracolsep{\fill}}r}
  \textbf{\Large Fedor Zhirkov} & Email : \href{mailto:fedorwoiwoi@gmail.comm}{fedorwoiwoi@gmail.com}\\
  Linkedin: \href{https://www.linkedin.com/in/fedor-zhirkov-3a6a83257/}{Fedor Zhirkov} & Mobile : +7\hspace{0.5ex}965\hspace{0.5ex}358\hspace{0.5ex}05\hspace{0.5ex}65 \\
\end{tabular*}


%-----------EDUCATION-----------------
\section{Education}
  \resumeSubHeadingListStart
    \resumeSubheading
       {National Research University Higher School of Economics}{Moscow, Russia}
      {Bachelor in Economics}{Sept. 2021 - June 2025}
      \begin{itemize}
          \item GPA: 8.5/10
          \item Main Courses: Calculus, Discrete maths*, Programming in python, Intelligent data analysis*, Databases*
          \item  * - are the projects, which I have studied from HSE Bachelor of Computer Science (Applied Mathematics and Informatics)
      \end{itemize}
  \resumeSubheading
       {Lyceum "Second School"}{Moscow, Russia}{Mathematics and Physics direction}{Sept. 2016 - June 2021}
    \resumeSubheading
      {School of Economics and Mathematics at Moscow State University}{Moscow, Russia}
      {Advanced Economics, Game Theory}{Sept. 2020 - June 2021 (Present)}
  \resumeSubHeadingListEnd


%-----------EXPERIENCE-----------------
\section{Experience}
  \resumeSubHeadingListStart
      \resumeExpSubheading
      {Gotbit (Venture Fund and Crypto-consulting company) }{St. Petersburg, Russia (remote)}
      {Junior Researcher Analyst}{June 2022 - Aug. 2022}
      {\skill{Financial modeling}\skill{Product analytics} \skill{Creating tokenomics} \skill{Business development} \skill{Risk assessment}}
      \resumeDesc{
      \begin{itemize}
          \item Analyzing and editing projects' inner business and financial model.
          \item Creating tokenomics for projects, adding new token utilities and analyzing its' benefits.
          \item Modeling game economy in {\href{https://machinations.io/}{Machinations}}.
          \item Successful leading projects from the fundraising stage to listing on Gate, KuCoin and other Exchanges. 
      \end{itemize}}
    
  \resumeSubHeadingListEnd

\section{Projects}
  \resumeSubHeadingListStart
  
      \resumeProjSubheading
      {Game Economy model in Machinations (under NDA till Aug. 2025)}{Moscow, Russia}
      {\skill{Product analytics} \skill{Risk assessment} \skill{Financial modeling}}{August 2020}
          \resumeDesc{Created a model for a web3.0 game project, which contains the mechanism of rewarding users with a token and token burning mechanism, simulation of game-processes, evaluation of game economy and visual representation of token's unlock}
  
      
  \resumeSubHeadingListEnd

\section{Achievements}
  \resumeSubHeadingListStart
    \resumeProjSubheading
      {Winner of Moscow School Olympiad in Economics}{Moscow, Russia}
      {\skill{Economics}}
      {May 2021}
    \resumeProjSubheading
      {Participant of the final stage of the All-Russian School Olympiad in Economics}{Russia}
      {\skill{Economics}}
      {April 2021}
    \resumeProjSubheading
      {Winner of the semi-final stage of the All-Russian School Olympiad in Maths and Economics}{Moscow, Russia}
      {\skill{Economics} \skill{Maths}}
      {Feb. 2020, Feb. 2021}
  \resumeSubHeadingListEnd
%
%--------PROGRAMMING SKILLS------------
\section{Programming Skills}
 \resumeSubHeadingListStart
   \item{
     \textbf{Languages}{: C++, Python}
   }\vspace{-7pt}
   \item{
     \textbf{Technologies}{: PostgreSQL, ORM, \LaTeX,}
   }
   \vspace{-7pt}
   \item{
     \textbf{Knowledge}{: JDBC, E-R modeling, A/B testing}
   }
 \resumeSubHeadingListEnd


%-------------------------------------------
\end{document}
