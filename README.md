# Lipreading-Audioless
 The task of generating textual descriptions from video
content presents a significant challenge, particularly when
audio is either absent or of poor quality. Traditional ap-
proaches have largely focused on lipreading techniques that
decode speech on a word-by-word basis. However, these
methods often fall short in accurately capturing the full
scope of spoken language. In our project, we explore the
implementation of lipnets, which employ a spatio-temporal
convolutional neural network (CNN) to process the visual
input derived from the mouth region’s movements. The
CNN’s output is then fed into a recurrent neural network
(RNN), which decodes the visual features into textual sen-
tences, bridging the gap between visual cues and linguistic
content. To achieve this task, we used an Extract of the orig-
inal GRID dataset ( high-quality audio and video (facial)
recordings of 1000 sentences spoken by each of 34 talkers
(18 male, 16 female), for a total of 34000 sentences. Sen-
tences are of the form ”put red at G9 now”). We train the
model with the video and annotations and evaluate its per-
formance relative to the original annotations using Connec-
tionist Temporal Classification (CTC) loss for the particular
video. We show that an end-to-end sentence-level lipread-
ing solution is attainable by this approach.
