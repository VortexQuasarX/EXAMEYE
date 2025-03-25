# EXAMEYE

\documentclass{article}
\usepackage{hyperref}

\title{Offline Exam Cheating Detection System}
\author{Your Name}
\date{\today}

\begin{document}

\maketitle

\section{Introduction}
The increasing incidence of cheating in academic examinations threatens the credibility of educational institutions, highlighting the need for effective monitoring systems. This project presents an \textbf{automated offline exam cheating detection system} leveraging advanced computer vision techniques to identify suspicious behaviors in real-time using CCTV footage.

\section{Features}
\begin{itemize}
    \item \textbf{YOLO-NAS}: Detects cheating behaviors, such as using unauthorized materials (e.g., mobile phones, papers).
    \item \textbf{YOLOv8}: Analyzes student actions, classifying behaviors into categories like daydreaming, normal, and stressed.
    \item \textbf{Real-time Monitoring}: The system processes live video feeds and triggers alerts when suspicious behavior is detected.
    \item \textbf{Multimodal Fusion}: Combines object detection with behavioral analysis for accurate and reliable monitoring.
    \item \textbf{Database Integration}: Stores detection results for review and accountability.
\end{itemize}

\section{Installation}
\subsection{Prerequisites}
Ensure you have the following installed:
\begin{itemize}
    \item Python (3.8+)
    \item OpenCV
    \item TensorFlow or PyTorch
    \item NumPy, Pandas, Matplotlib
    \item Flask (for web-based monitoring)
    \item FFmpeg (for video processing)
\end{itemize}

\subsection{Setup}
\begin{verbatim}
git clone https://github.com/yourusername/cheating-detection-system.git
cd cheating-detection-system
pip install -r requirements.txt
\end{verbatim}

\section{Usage}
\subsection{Running the System}
To start real-time monitoring:
\begin{verbatim}
python main.py
\end{verbatim}

To process recorded video:
\begin{verbatim}
python detect_cheating.py --video input_video.mp4
\end{verbatim}

\subsection{Training Models}
Train YOLO-NAS for cheating detection:
\begin{verbatim}
python train.py --model yolonas --dataset data/cheating_dataset
\end{verbatim}

Train YOLOv8 for behavior analysis:
\begin{verbatim}
python train.py --model yolov8 --dataset data/behavior_dataset
\end{verbatim}

\section{Evaluation Metrics}
The model's performance is evaluated using:
\begin{itemize}
    \item \textbf{Mean Average Precision (mAP)}: 74.9\%
    \item \textbf{Precision}: 73.9\%
    \item \textbf{Recall}: 82.4\%
    \item \textbf{F1-Score}: Balanced metric for accuracy
\end{itemize}

\section{Future Improvements}
\begin{itemize}
    \item Enhance detection accuracy by refining training datasets.
    \item Improve false-positive filtering using advanced data fusion.
    \item Implement facial recognition for student verification.
    \item Develop a detailed reporting system for detected cheating incidents.
\end{itemize}

\section{License}
This project is licensed under the MIT License. See the LICENSE file for details.

\section{Contributing}
Contributions are welcome! Feel free to open an issue or submit a pull request.

\section{Contact}
For questions or support, contact \href{mailto:your.email@example.com}{your.email@example.com}.

\end{document}
