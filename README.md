## Bahareh Toushkan

Computer science undergraduate at Seoul National University, graduating February 2027.
I work across systems programming and applied AI, and two questions keep pulling me in:

- **Checking AI-written code.** I build software with an AI coding agent, and I keep
  asking how we can check that the code it writes is actually safe.
- **Reading neural signals.** Moving toward computational neuroscience — reading neural
  and physiological signals well enough to act on them.

**Systems work** (coursework in C; course code is not public)

- Concurrent key–value store server: 10 worker threads over TCP, per-bucket reader–writer
  locks built from one mutex and one condition variable, FIFO ordering. I used an AI
  assistant to cross-check my lock-ordering logic and to help find a deadlock, then
  verified the rest against the reference server myself.
- Software router: longest-prefix-match forwarding, ARP, ICMP and a subnet blacklist
- Heap manager replacing `malloc`/`free`, and a Unix shell with job control and signal handling
- X.509 certificate validation with OpenSSL, including OCSP revocation checks
- 8-bit microprocessor on an FPGA in Verilog (team project)

**Applied AI and neuroscience**

I came to neuroscience from a project rather than from coursework. In a four-person team I
designed **Roya**, a closed-loop sleep-care system that detects physiological states
associated with nightmares and intervenes with low-intensity bone-conduction
stimulation without waking the sleeper. The result I keep returning to is a failure:
identifying REM from autonomic signals alone gave **AUC 0.522** — chance — which is
what forced a two-stage architecture with an EEG gate ahead of the autonomic model.
The stage that worked reached **AUC 0.816** on DREAMT under subject-wise
cross-validation.

**What I'm interested in**

- How to check that software an AI agent wrote is safe
- Reading sleep and neural state reliably enough to intervene at the right moment
- Decision-making and reinforcement learning as models of behaviour
- Assistive technology — ADHD support tools, and brain-machine interfaces for
  people with spinal cord injury

**Repositories**

| | |
| --- | --- |
| [eeg-sleep-staging](https://github.com/bahareh-toushkan/eeg-sleep-staging) | Sleep-stage classification from two-channel EEG. Shows why accuracy is the wrong metric here: 0.87 accuracy, 0.70 macro-F1, and an N1 F1 of 0.38. |
| [drift-diffusion-model](https://github.com/bahareh-toushkan/drift-diffusion-model) | The drift-diffusion model of decisions, implemented from the first-passage density up, with likelihood validation against simulation and parameter recovery (r > 0.98). |

**Currently**

Writing an undergraduate thesis on how humans and language models resolve ambiguous
romanised Persian — reaction times and confidence ratings analysed with mixed-effects
models, the identical stimuli run through five language models. Also building a
schedule-and-reminder app with an AI coding agent, which is where the code-safety
question came from, and working through the [Neuromatch Academy computational
neuroscience curriculum](https://compneuro.neuromatch.io/).

**Background**

Two-month research internship at SNU building an empirical dataset of polarized
magnetic field distributions in three-dimensional space; the measurements were later
used in a joint research proposal with the Korea Research Institute of Standards and
Science.

C, OpenSSL, POSIX threads, Verilog · Python, PyTorch, XGBoost, scikit-learn, numpy/scipy.
Persian (native), Korean (TOPIK 6), English.

Reach me at 2022-16032@snu.ac.kr
