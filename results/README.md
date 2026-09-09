# Results and Signal Captures

This page records what can be read directly from the supplied project images. The original filenames use the project name **Chronisense**.

## Confusion Matrix

![Original confusion matrix with true labels on rows and predicted labels on columns](confusion-matrix.png)

The original PNG has a transparent background. Its black axis text may be difficult to read in a dark theme; the table below preserves the labels and values.

| True label \ Predicted label | No Pain | Pain | Row total |
| --- | ---: | ---: | ---: |
| No Pain | 155 | 8 | 163 |
| Pain | 30 | 149 | 179 |
| Column total | 185 | 157 | 342 |

The four displayed cells sum to 342. The diagonal contains 304 entries and the off-diagonal contains 38. These totals are arithmetic derived from the exported image; they do not identify the observation unit or establish an independent test set.

Before reporting detection performance, document:

- **TODO:** What each matrix entry represents: sample, time window, episode, participant, or another unit.
- **TODO:** How the reference labels “No Pain” and “Pain” were assigned.
- **TODO:** Who or what was measured, under what conditions, and over what duration.
- **TODO:** Which algorithm, preprocessing settings, and thresholds produced these predictions.
- **TODO:** Whether threshold development and evaluation used separate data.
- **TODO:** How repeated or correlated observations were handled.
- **TODO:** The underlying records and script needed to reproduce the figure.

Generalization to new participants and clinical performance remain unverified.

## EMG Display Captures

![First EMG display capture](../images/emg-display-01.png)

![Second EMG display capture](../images/emg-display-02.png)

Both screenshots show an orange trace with **EMG** selected and **ECG** unselected. They show numerical axes but no axis titles or units. The captures display different numerical ranges; the images alone do not establish their physical units, timing, filtering, calibration, or muscle-activity conditions.

- **TODO:** Identify the plotting application and source-data format.
- **TODO:** Define both axes and the acquisition rate.
- **TODO:** State whether the plotted values are raw ADC readings, conditioned sensor output, or a computed feature.
- **TODO:** Describe electrode placement, capture conditions, and any preprocessing.
- **TODO:** Add corresponding raw data and timestamps if available.
- **TODO:** Add an ECG capture and an annotated detection event if available.

The captures' muscle-activity conditions and time units remain unconfirmed.

## Media Provenance

| Repository asset | Supplied original filename |
| --- | --- |
| `confusion-matrix.png` | `Chronisense Confusion Matrix.png` |
| `../images/emg-display-01.png` | `Chronisense muscle tension plot.png` |
| `../images/emg-display-02.png` | `Chronisense muscle tension plot 2.png` |
| `../media/muscle-tension-demo.mp4` | `Chronisense muscle tension demo.MOV` |

The filenames are normalized for repository use. The PNGs preserve the supplied images. The video is transcoded to MP4 for browser playback, with embedded metadata removed.
