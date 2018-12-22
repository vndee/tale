---
layout: post
title: '[NMZD #03] How does LSTM network work efficiently?'
author: Duy Huynh
published: true
---
From qoura: [How does LSTM network work efficiently?](https://www.quora.com/How-does-LSTM-network-work-efficiently)

Rishi Bommasani:

So it is not clear what the word efficiency means contextually. In terms of run-time, the asymtopic run times will all be the same as the classical RNN counterparts, which we usally don't care about for practical applications of LSTMs. In practice, the idea of keeping this memory unit for LSTMs that isn't present in RNNs in the same sense is not a major computational concern, and really they are the reason why LSTMs are effective, as this is the major innovation over classical RNNs. LSTMs can leverage past information (and bi-directional LSTMs leverage future information by working in the reverse direction as well) in generating output. This can for the majority of tasks be a problem, as intuitively this is not how the task is done (say by a human). However, for a task like predicting the next word in a setence, an LSTM model is very sensible, as the previous text (beyond say the previous word) will have a large effect on what is and isn't reasonable prediction/output.
