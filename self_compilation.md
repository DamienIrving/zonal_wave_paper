In order to self compile this document using pdflatex, export the zip file and then
do the following:  

1. Change the document formatting section to:

\documentclass[a4paper,12pt]{article}

```
%% Load packages %%

% Line and page formating %
\usepackage{setspace}          % Line spacing
\onehalfspacing 
\usepackage{lineno}           % Line numbering
\linenumbers
\usepackage{enumerate}         % Numbered lists
  
% Figures %
\usepackage{graphicx}          % Include graphics in document (enables \includegraphics command)
\usepackage{ccaption}          % Figure and table captions
%\usepackage{subfigure}         % Allows figures side by side (might be outdated and replaced with subfig)
%\usepackage{rotating}          % Rotation of figures
\usepackage[nomarkers,figuresonly]{endfloat}   % Move all figures to end of document

% Indexing, labelling and citations %
\usepackage{makeidx} 
\usepackage{natbib}            % Advanced version of \cite; allows in text (\citet) and in parentheses (\citep) referencing
\usepackage[capitalise]{cleveref}   % For referencing equations and figures    % to use noabbrev option, I'll need an updated installation of cleveref

% Maths %
\usepackage{amssymb,amsmath}

```

2. Change the referencing style (near the beginning of the file)

```\bibliographystyle{bibliography/agu_ed} ```


3. Change the bibliography reference (at end of file)

```\bibliography{bibliography/biblio}```