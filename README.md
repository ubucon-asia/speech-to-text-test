# Testing Google Speech-To-Text subtitle generation.

This repo is for gathering results of testing Closed caption generation using Google speech to text.

## To test:
- Prepare a video file with following details:
    - A video of tech conference session recordings
    - Video length: about 10~30minutes
    - Language: Your local language (e.g. Korean, Japanese, Chinese, Cantonese, etc…)
- Use PyTranscriber or speech2srt tutorial and generate subtitle from the prepared video
    - Google Cloud - speech2srt tutorial: https://cloud.google.com/community/tutorials/speech2srt
        - Requires Google cloud account
        - First 60minutes free, more usage will be charged.
    - pyTranscriber: https://github.com/raryelcostasouza/pyTranscriber
- Try playing video with generated subtitle
- While watching the video, check every typos from the subtitles.
- Make a copy of the subtitle, fix typos from the copy of the subtitle file.

## Submitting test report
- Create directory for the video you tested.
- Add markdown file to describe test result
- Commit original subtitle first. (e.g. `myvideo/subtitle_name.srt`)
- Make a copy of original on same path and change file extension with `.original.srt` (e.g. `myvideo/subtitle_name.original.srt`)
- Overwrite original one without `.original.srt` with your modified subtitle
- Commit and push updated files.

## Notes:
- This test is to see how many efforts are required for future volunteers to work on video subtitles.
- You don’t need to choose a long video to test. If you are busy with other things, testing a 10minutes video is totally ok.
- For now, you can just test speech-to-text only. If you want, you can also try using Translation API to see machine translation quality.
- In case, when you’re too busy to fix typos from generated subtitles, you may just count the number of total typos.
- If it’s very easy to gather speakers who are fluent in English from your region. Since the purpose of working on subtitles is to help engage speakers who are not fluent with English, You may not need to test things related with subtitles. Please let me know in that case.
- Complete test until next sunday (March 14th) midnight in your timezone. If you need more time to work on testing, please let me know.
