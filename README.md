## Bahareh Toushkan

Computer science undergraduate at Seoul National University, graduating February 2027.
Moving toward computational neuroscience — reading neural and physiological signals
well enough to act on them.

I came to this from a project rather than from coursework. In a four-person team I
designed **Roya**, a closed-loop sleep-care system that detects physiological states
associated with nightmares and intervenes with low-intensity bone-conduction
stimulation without waking the sleeper. The result I keep returning to is a failure:
identifying REM from autonomic signals alone gave **AUC 0.522** — chance — which is
what forced a two-stage architecture with an EEG gate ahead of the autonomic model.
The stage that worked reached **AUC 0.816** on DREAMT under subject-wise
cross-validation.

**What I'm interested in**

- Reading sleep and neural state reliably enough to intervene at the right moment
- Decision-making and reinforcement learning as models of behaviour
- Assistive technology — ADHD support tools, and brain-machine interfaces for
  people with spinal cord injury

**Repositories**

| | |
| --- | --- |
| [eeg-sleep-staging](../../../eeg-sleep-staging) | Sleep-stage classification from two-channel EEG. Shows why accuracy is the wrong metric here: 0.87 accuracy, 0.70 macro-F1, and an N1 F1 of 0.38. |
| [drift-diffusion-model](../../../drift-diffusion-model) | The drift-diffusion model of decisions, implemented from the first-passage density up, with likelihood validation against simulation and parameter recovery (r > 0.98). |

**Currently**

Working through the [Neuromatch Academy computational neuroscience
curriculum](https://compneuro.neuromatch.io/), and writing an undergraduate thesis on
how humans and language models resolve ambiguous romanised Persian — reaction times
and confidence ratings analysed with mixed-effects models, the identical stimuli run
through five language models.

**Background**

Two-month research internship at SNU building an empirical dataset of polarized
magnetic field distributions in three-dimensional space; the measurements were later
used in a joint research proposal with the Korea Research Institute of Standards and
Science.

Python, PyTorch, XGBoost, scikit-learn, numpy/scipy. Korean (TOPIK 6), English, Persian.

Reach me at 2022-16032@snu.ac.kr
