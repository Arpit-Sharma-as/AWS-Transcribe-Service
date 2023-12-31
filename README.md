# AWS Transcription Script

This Python script utilizes the AWS Transcribe service to transcribe audio files. It uses the Boto3 library to interact with AWS services.

## Prerequisites

- Python installed on your machine
- Boto3 library (`pip install boto3`)
- AWS credentials configured on your machine
- An audio file in an S3 bucket that you want to transcribe

## Usage

1. Clone the repository:

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Install the required Python packages:

    ```bash
    pip install boto3
    ```

3. Run the script:

    ```bash
    python transcribe_audio.py
    ```

4. The script will prompt you for the S3 URI of the audio file to transcribe.

5. The transcription job will be started, and the script will wait for its completion.

6. Once the transcription is complete, the script will download the transcript and save it to a text file.

## Configuration

- Open the script (`transcribe_audio.py`) and modify the following variables:
    - `input_audio_path`: The S3 URI of your input audio file.
    - `output_text_path`: The local path to save the transcribed text.

## Notes

- Ensure that your AWS credentials are properly configured on your machine.
- The language and media format for transcription can be modified in the script.
- The script waits for the transcription job to complete, so it may take some time depending on the audio file's length.
