.. _Preparing a Video:

#########################
Preparing a Video
#########################


Before you add a video to a course, you need the following items.

* A place to :ref:`host<Set Up a Hosting Service>`, or store, your videos.
* A video that meets the recommended :ref:`specifications<REFERENCE>`.
* A :ref:`transcript<Obtain a Video Transcript>` in SubRip Text (.srt) format
  for the video.

.. contents::
 :local:
 :depth: 1

************************
Set Up a Hosting Service
************************

.. only:: Partners

  .. note
    For courses on edx.org, you do not have to set up a hosting service to
    store your videos. You can skip to the :ref:`Create a Video` section.

    For Edge courses, you must work with a third party hosting site to make
    your videos available for streaming or download.

.. only:: Open_edX

  You must work with a third party hosting site to make your videos available
  for streaming or download.

You can use any video hosting site that you want. Many courses use Amazon S3.
When you select a video hosting site, we strongly recommend that you keep the
following information in mind.

* The hosting site might have to handle high traffic volume.
* Not all hosting sites are available in all countries or regions. We recommend
  that you upload videos to more than one hosting site.
* Learners' internet connections vary widely. We recommend that you make your
  videos available for both download and streaming.
* The URL for your videos must end in .mp4, .mpeg, .webm, or .ogg. The video
  player cannot support videos that you upload on sites such as Vimeo.

  .. note::
    To help make sure all standard browsers can play your video, we strongly
    recommend that you use .mp4 format.

.. _Create the Video:

******************************
Create a Video
******************************

Your videos can contain whatever content you want to include in the course. The
following resources can help you to create good video content that is based on
extensive experimental research in student learning.

* The `Creating Videos`_ section of `Overview of Creating an edX Course`_
* Richard E. Mayer's `12 Principles of Multimedia Learning`_

.. _Compression Specifications:

When you create video files, keep the following guidelines in mind.

.. contents::
 :local:
 :depth: 1

==============================
General Guidelines
==============================

* Videos should be as short as possible. Learners are more likely to finish
  watching videos that are no more than 5-10 minutes long.
* Each video file that you upload must be less than 5GB in size.
* Each video should follow established :ref:`file naming conventions <File
  Naming Conventions>` and :ref:`video compression specifications <Video
  Compression Specifications>`.
* The video player supports videos in .mp4, .mpeg, .webm, and .ogg format.
  However, to help make sure all standard browsers can play your video, we
  **strongly** recommend that you use the .mp4 format.

.. only:: Partners

  For courses on edx.org, your videos must use the .mp4 or .mov format. For
  more information, see Uploading Videos in Studio.

  For courses on Edge, we strongly recommend that you create additional copies
  of your videos in the following resolutions to provide the best possible
  experience for learners who are using different devices. When multiple videos
  are available, the video player automatically plays the best video for each
  learner's device and internet connection.

.. only:: Open_edX

  Additionally, we strongly recommend that you create copies of your videos in
  the following resolutions to provide the best possible experience for
  learners who are using different devices. When multiple resolutions are
  available, the video player automatically plays the best video for each
  learner's device and internet connection.

* 1080p
* 720p
* Mobile 360p

.. _File Naming Conventions:

=======================
File Naming Conventions
=======================

Each video file must have a unique name. We strongly recommend that
organizations define a naming convention for video files, and use that
convention in videos for all courses to facilitate identifying and tracking
video files.

At a minimum, your naming convention should include these elements.

* A course identifier.
* The year of the initial course run.
* A revision or version number.

For example, you might use the following naming convention.

::

  {course number}_{year}_{section}_{subsection}_{unit}_{version}.{type}

This convention might yield the following file name.

::

  SPU27_2015_S1_SS3_U4_v2.mp4

.. note::
  Include only alphanumeric characters and underscores in video file names. Do
  not use periods except for the period before the file name extension (for
  example, .mp4).


.. _Video Compression Specifications:

=================================
Video Compression Specifications
=================================

only:: Partners

  For courses on edx.org, all videos must comply with the following
  specifications.

  For courses on Edge, the following video compression specifications are
  strongly recommended, but not required.

only:: Open_edX

  The following video compression specifications are strongly recommended, but
  not required.


.. list-table::
   :widths: 10 20 20
   :stub-columns: 1

   * - :ref:`Codec<codec_g>`
     - H.264 .mp4
   * - Resolution & Frame Rate
     - 1280x720, progressive, 29.97 fps

       .. note::
         Typically, you export at the same frame rate that was used when you
         created the media file. For example, if you create the file in a
         country that uses the :ref:`PAL<PAL>` system, you export at 25 fps
         instead of the :ref:`NTSC<NTSC>` standard of 29.97 fps.

   * - Aspect
     - 1.0
   * - Bit Rate
     - VBR, 2 pass
   * - Target :ref:`VBR<VBR>`
     - 1 mbps
   * - Max :ref:`VBR<VBR>`
     - 1.5 mbps
   * - Audio
     - :ref:`AAC<AAC>` 44.1 / 192 kbps

******************************
Obtain a Video Transcript
******************************

Transcripts are required for all videos. Transcripts help learners with
hearing impairments understand audio content, and they are helpful for learners
who speak other languages.

Transcripts are available to learners in the following ways.

* Learners can select the **Show transcript** (”) icon in the video player’s
  control bar to show the transcript next to the video. The transcript
  automatically scrolls as the video plays. Learners can select a line in the
  transcript to jump to the point in the video where that line is spoken.
* Learners can show the transcript file as overlaid closed captions for the
  video by selecting the **CC** icon in the video player’s control bar.
* You can allow learners to download transcripts so that they can read them
  offline. For more information, see :ref:`REFERENCE`.

=============================
Obtaining a Video Transcript
=============================

.. only:: Partner

  For courses on edx.org, transcripts must be in the SubRip Text (.srt) format.
  For courses on Edge, we strongly recommend that you obtain timed transcripts
  in the .srt format.

  To obtain a transcript in .srt format, you can work with a transcript
  provider such as `3Play Media`_ or `cielo24`_. 3Play Media and cielo24 offer
  a discounted rate for edX partners.

  Additionally, if your course is on edx.org and you work with 3Play Media or
  cielo24, you can use integrated video transcripts in Studio to obtain
  transcripts and associate them with your videos automatically. For more
  information, see :ref:`Integrated Transcripts`.

  If your course is on Edge, or you do not work with 3Play Media or cielo24,
  you must obtain transcripts from a third party transcript provider and
  associate them with your videos manually. For more information, see :ref:`Non
  Integrated Transcripts`.

  .. note::
    If you use a third party transcript provider other than 3Play Media or
    cielo24, make sure that your finished transcripts are in .srt format.


  Integrated Transcripts
  **********************

  When you use integrated transcripts, you upload your videos in Studio. The
  edX processing service then creates transcripts, uploads the transcripts, and
  links the transcripts with your videos automatically. For more information,
  see <LINK TO INFO ABOUT VIDEO PROCESSING SERVICE>.

  To set up integrated video transcripts, follow these steps.

  .. note::
    Usually, transcript providers establish accounts with organizations instead
    of with course teams. Check with your organization to see if the
    organization has an account with 3Play Media or cielo24.

  #. Contact either 3Play Media or cielo24, and specify that you are an edX
     partner.

     3Play Media or cielo24 give you credentials that you then enter in Studio.

  #. When you receive account credentials from 3Play Media or cielo24, open
     your course in Studio, and then select **Video Uploads** on the
     **Content** menu.

  #. On the **Video Uploads** page, locate **Course Video Settings**.

  #. In the Course Video Settings panel, specify the information for your
     organization.

     .. important::
      If these settings have already been specified, do not change them. If
      your course uses a different company or different account, contact your
      organization's administrator.

     * If your organization uses 3Play Media, select 3Play Media under
       Automated Transcripts, and then enter your API key and secret key. When
       you have entered this information, select Update Settings.

     * If your organization uses cielo24, select cielo24 under Automated
       Transcripts, enter your API key, and then select Update Settings.


  Non-Integrated Transcripts
  **************************

  If you work with a transcript provider other than 3Play Media or cielo24, or
  your course is on Edge, you cannot use the integrated video transcript
  functionality in Studio. Instead, you send your videos to the transcript
  provider, and the provider sends you the completed transcripts. You later
  upload the transcripts when you :ref:`create a video component<Create a Video
  Component>`.

  If your course is on Edge, you must follow the process for non-integrated
  transcripts even if you work with 3Play Media or cielo24.

.. only:: Open_edX

  When you work with a transcript provider, you send your videos to the
  transcript provider, and the provider sends you the completed transcripts.
  You later upload the transcripts when you :ref:`create a video
  component<Create a Video Component>`.

=====================================
Transcript File Naming Conventions
=====================================

To prevent errors when you upload your video transcripts, we recommend the
following conventions for naming your transcript files.

.. only:: Partners

  .. note::
    If your course uses integrated video transcripts, the edX video processing
    service names your transcripts automatically. For more information, see
    :ref:`Integrated Video Transcripts`.


* Give each transcript file an identifying name that is unique across all of
  your course uploads, including non-transcript files.
* Make sure that the transcript contains no special characters, such as ç, å,
  or ó.
* Make sure that the file type, `.srt`, is in lowercase.
* Do not include periods in file names other than the period before the .srt
  file type.



.. include:: ../../../links/links.rst
