# Pulsar Validator
This program works in two modes:
1. Compare the positive and negative output of [PulsarClassifier](https://github.com/jacob-ian/PulsarClassifier) to the list of known pulsars.
1. Create a list of the feature extracted pulsars.

## Requirements
* Java 1.6 or later
* Pulsar classification test candidate data
  * A list of the pulsars included in the data set (one candidate per line)
* Outputs from [PulsarClassifier](https://github.com/jacob-ian/PulsarClassifier).

## Usage
1. Download the file `pulsarvalidator-1.0-full.jar` located inside the `target` directory of this repository.
1. Run the command:
```
$ java -jar pulsarvalidator-1.0-full.jar -v [PATH TO LIST OF PULSARS] [PATH TO .POSITIVE CLASSIFIER OUTPUT] [PATH TO .NEGATIVE CLASSIFIER OUTPUT]
```

## Output
This program will output the following statistics:
* Number of Pulsars
* Number of Detected Pulsars
* True Positives
* False Positives
* Number of Non-Pulsars
* Number of Detected Non-Pulsars
* True Negatives
* False Negatives

## License
This software is produced under the GNU General Public License Version 3.