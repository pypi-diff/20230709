# Comparing `tmp/pywa-0.0.1rc16-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc17-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,23 @@
-Zip file size: 28295 bytes, number of entries: 15
+Zip file size: 32701 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      117 b- defN 23-Jun-27 07:52 pywa/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-07 08:22 pywa/__version__.py
--rw-rw-r--  2.0 unx    14991 b- defN 23-Jul-03 08:35 pywa/api.py
--rw-rw-r--  2.0 unx    26847 b- defN 23-Jul-03 08:42 pywa/client.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-09 17:47 pywa/__version__.py
+-rw-rw-r--  2.0 unx    14468 b- defN 23-Jul-09 17:38 pywa/api.py
+-rw-rw-r--  2.0 unx    29314 b- defN 23-Jul-09 17:43 pywa/client.py
 -rw-rw-r--  2.0 unx     7191 b- defN 23-Jul-03 08:28 pywa/errors.py
--rw-rw-r--  2.0 unx    20703 b- defN 23-Jul-04 19:49 pywa/filters.py
+-rw-rw-r--  2.0 unx    21225 b- defN 23-Jul-09 17:29 pywa/filters.py
 -rw-rw-r--  2.0 unx     1794 b- defN 23-Jul-02 08:19 pywa/handlers.py
--rw-rw-r--  2.0 unx    39628 b- defN 23-Jul-07 08:18 pywa/types.py
--rw-rw-r--  2.0 unx      991 b- defN 23-Jun-20 16:58 pywa/utils.py
--rw-rw-r--  2.0 unx     4613 b- defN 23-Jul-03 08:35 pywa/webhook.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-07 08:22 pywa-0.0.1rc16.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4387 b- defN 23-Jul-07 08:22 pywa-0.0.1rc16.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 08:22 pywa-0.0.1rc16.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-07 08:22 pywa-0.0.1rc16.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1106 b- defN 23-Jul-07 08:22 pywa-0.0.1rc16.dist-info/RECORD
-15 files, 123557 bytes uncompressed, 26513 bytes compressed:  78.5%
+-rw-rw-r--  2.0 unx      873 b- defN 23-Jul-09 12:48 pywa/utils.py
+-rw-rw-r--  2.0 unx     4449 b- defN 23-Jul-09 13:09 pywa/webhook.py
+-rw-rw-r--  2.0 unx      336 b- defN 23-Jul-07 13:20 pywa/types/__init__.py
+-rw-rw-r--  2.0 unx     9301 b- defN 23-Jul-09 17:41 pywa/types/base_update.py
+-rw-rw-r--  2.0 unx     5653 b- defN 23-Jul-07 13:38 pywa/types/callback.py
+-rw-rw-r--  2.0 unx     4609 b- defN 23-Jul-09 14:47 pywa/types/media.py
+-rw-rw-r--  2.0 unx    11234 b- defN 23-Jul-09 17:38 pywa/types/message.py
+-rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-07 13:28 pywa/types/message_status.py
+-rw-rw-r--  2.0 unx     9156 b- defN 23-Jul-07 13:38 pywa/types/others.py
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-09 17:47 pywa-0.0.1rc17.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4420 b- defN 23-Jul-09 17:47 pywa-0.0.1rc17.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-09 17:47 pywa-0.0.1rc17.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-09 17:47 pywa-0.0.1rc17.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-09 17:47 pywa-0.0.1rc17.dist-info/RECORD
+21 files, 128854 bytes uncompressed, 30175 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -15,32 +15,50 @@
 
 Filename: pywa/filters.py
 Comment: 
 
 Filename: pywa/handlers.py
 Comment: 
 
-Filename: pywa/types.py
-Comment: 
-
 Filename: pywa/utils.py
 Comment: 
 
 Filename: pywa/webhook.py
 Comment: 
 
-Filename: pywa-0.0.1rc16.dist-info/LICENSE
+Filename: pywa/types/__init__.py
+Comment: 
+
+Filename: pywa/types/base_update.py
+Comment: 
+
+Filename: pywa/types/callback.py
+Comment: 
+
+Filename: pywa/types/media.py
+Comment: 
+
+Filename: pywa/types/message.py
+Comment: 
+
+Filename: pywa/types/message_status.py
+Comment: 
+
+Filename: pywa/types/others.py
+Comment: 
+
+Filename: pywa-0.0.1rc17.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc16.dist-info/METADATA
+Filename: pywa-0.0.1rc17.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc16.dist-info/WHEEL
+Filename: pywa-0.0.1rc17.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc16.dist-info/top_level.txt
+Filename: pywa-0.0.1rc17.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc16.dist-info/RECORD
+Filename: pywa-0.0.1rc17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1rc16"
+__version__ = "0.0.1rc17"
```

## pywa/api.py

```diff
@@ -1,10 +1,13 @@
+import io
 import mimetypes
 import requests
-from typing import Iterable
+from typing import Iterable, BinaryIO
+from requests_toolbelt import MultipartEncoder
+
 from pywa.errors import WhatsAppError
 from pywa.types import InlineButton, SectionList, Contact
 
 
 class WhatsAppCloudApi:
     """Internal methods for the WhatsApp client."""
 
@@ -98,63 +101,52 @@
             method="POST",
             endpoint=f"/{self.phone_id}/messages",
             json=data
         )
 
     def upload_media(
             self,
-            media: str | bytes,
-            mime_type: str | None
+            media: bytes | BinaryIO,
+            mime_type: str,
+            file_name: str = "file",
     ) -> dict[str, str]:
         """
         Upload a media file to WhatsApp.
 
         Return example::
 
             {
               'id':'<MEDIA_ID>'
             }
 
         Args:
-            media: media bytes / path / URL to upload.
-            mime_type: The type of the media file (if not provided, it will be guessed with the `mimetypes` library).
-
+            media: media bytes or open(path, 'rb') object
+            mime_type: The type of the media file
+            file_name: The name of the media file (default: ``file``).
         Returns:
             A dict with the ID of the uploaded media file.
-
-        Raises:
-            ValueError: If ``mime_type`` is not provided and cannot be guessed (e.g. for bytes or URLs without
-             ``Content-Type`` header).
         """
-        if isinstance(media, str):
-            if media.startswith(("https://", "http://")):
-                res = requests.get(media)
-                res.raise_for_status()
-                file = res.content
-                mime_type = mime_type or res.headers.get('Content-Type', default=res.headers.get('content-type'))
-            else:
-                mime_type = mime_type or mimetypes.guess_type(media)[0]
-                with open(media, "rb") as f:
-                    file = f.read()
-        else:
-            file = media
-        if mime_type is None:
-            raise ValueError("mime_type is required")
         headers = self._session.headers.copy()
-        headers["Content-Type"] = mime_type
-        files = {
-            'file': (None, file),
-            'type': (None, mime_type),
-            'messaging_product': (None, '"whatsapp"'),
-        }
+        form_data = MultipartEncoder(
+            {
+                "file": (
+                    file_name,
+                    media,
+                    mime_type
+                ),
+                "messaging_product": "whatsapp",
+                "type": mime_type
+            }
+        )
+        headers["Content-Type"] = form_data.content_type
         return self._make_request(
             method="POST",
             endpoint=f"/{self.phone_id}/media",
             headers=headers,
-            files=files
+            data=form_data
         )
 
     def get_media_url(self, media_id: str) -> dict:
         """
         Get the URL of a media file.
             - The url is valid for 5 minutes and can be downloaded only with access token.
             - For more info: https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#retrieve-media-url
```

## pywa/client.py

```diff
@@ -2,15 +2,15 @@
 
 __all__ = ("WhatsApp",)
 
 import hashlib
 import mimetypes
 import os
 import requests
-from typing import Callable, Any, Iterable
+from typing import Callable, Any, Iterable, BinaryIO
 from pywa.api import WhatsAppCloudApi
 from pywa.handlers import Handler, MessageHandler, ButtonCallbackHandler, SelectionCallbackHandler, RawUpdateHandler, \
     MessageStatusHandler
 from pywa.types import InlineButton, SectionList, Message, CallbackButton, CallbackSelection, MessageStatus, Contact, \
     MediaUrlResponse
 from pywa.webhook import Webhook
 
@@ -274,18 +274,43 @@
                 "type": "text",
                 "text": header,
             } if header else None,
             body=text,
             footer=footer,
         )['messages'][0]['id']
 
+    send_text = send_message  # alias
+
+    def _resolve_media_param(
+            self,
+            media: str | bytes | BinaryIO,
+            mime_type: str,
+            file_name: str,
+    ) -> tuple[bool, str]:
+        """
+        Internal method to resolve media parameters to a media ID or URL.
+        """
+        if isinstance(media, str):
+            if media.startswith(("https://", "http://")):
+                return True, media
+            elif not os.path.isfile(media) and media.isdigit():
+                return False, media  # assume it's a media ID
+            else:
+                return False, self.upload_media(
+                    media=media,
+                    mime_type=mimetypes.guess_type(media)[0] or mime_type,
+                    file_name=os.path.basename(media) or file_name
+                )
+        else:
+            return False, self.api.upload_media(media=media, mime_type=mime_type, file_name=file_name)['id']
+
     def send_image(
             self,
             to: str,
-            image: str | bytes,
+            image: str | bytes | BinaryIO,
             caption: str | None = None,
             reply_to_message_id: str | None = None,
             buttons: list[InlineButton] | None = None,
             body: str | None = None,
             footer: str | None = None,
     ) -> str:
         """
@@ -297,24 +322,25 @@
             ...     to="1234567890",
             ...     image="https://example.com/image.png",
             ...     caption="This is an image!",
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
-            image: The image to send (either a URL or a file ID).
+            image: The image to send (either a media ID, URL, file path, bytes, or a open file object).
             caption: The caption of the image (optional, markdown allowed).
             reply_to_message_id: The message ID to reply to (optional).
             buttons: The buttons to send with the image (optional).
             body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).
             footer: The footer of the message (if buttons is provided, optional, markdown has no effect).
 
         Returns:
             The message ID of the sent image.
         """
+        is_url, image = self._resolve_media_param(media=image, mime_type="image/jpeg", file_name="image.jpg")
         if not buttons:
             return self.api.send_media(
                 to=to,
                 media_id_or_url=image,
                 media_type="image",
                 reply_to_message_id=reply_to_message_id,
                 caption=caption,
@@ -323,26 +349,26 @@
             raise ValueError("Either body or caption must be provided when sending an image with buttons.")
         return self.api.send_interactive_message(
             to=to,
             keyboard=buttons,
             header={
                 "type": "image",
                 "image": {
-                    "link" if image.startswith(("https://", "http://")) else "id": image,
+                    "link" if is_url else "id": image,
                 }
             },
             body=body or caption,
             footer=footer,
             reply_to_message_id=reply_to_message_id,
         )['messages'][0]['id']
 
     def send_video(
             self,
             to: str,
-            video: str | bytes,
+            video: str | bytes | BinaryIO,
             caption: str | None = None,
             reply_to_message_id: str | None = None,
             buttons: list[InlineButton] | None = None,
             body: str | None = None,
             footer: str | None = None,
     ) -> str:
         """
@@ -354,24 +380,25 @@
             ...     to="1234567890",
             ...     video="https://example.com/video.mp4",
             ...     caption="This is a video",
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
-            video: The video to send (either a URL or a file ID).
+            video: The video to send (either a media ID, URL, file path, bytes, or a open file object).
             caption: The caption of the video (optional, markdown allowed).
             reply_to_message_id: The message ID to reply to (optional).
             buttons: The buttons to send with the video (optional).
             body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).
             footer: The footer of the message (if buttons is provided, optional, markdown has no effect).
 
         Returns:
             The message ID of the sent message.
         """
+        is_url, video = self._resolve_media_param(media=video, mime_type="video/mp4", file_name="video.mp4")
         if not buttons:
             return self.api.send_media(
                 to=to,
                 media_id_or_url=video,
                 media_type="video",
                 reply_to_message_id=reply_to_message_id,
                 caption=caption,
@@ -380,120 +407,123 @@
             raise ValueError("Either body or caption must be provided when sending a video with buttons.")
         return self.api.send_interactive_message(
             to=to,
             keyboard=buttons,
             header={
                 "type": "video",
                 "video": {
-                    "link" if video.startswith(("https://", "http://")) else "id": video,
+                    "link" if is_url else "id": video,
                 }
             },
             body=body or caption,
             footer=footer,
             reply_to_message_id=reply_to_message_id,
         )['messages'][0]['id']
 
     def send_document(
             self,
             to: str,
-            document: str | bytes,
-            filename: str | None = None,
+            document: str | bytes | BinaryIO,
+            file_name: str | None = None,
             caption: str | None = None,
             reply_to_message_id: str | None = None,
             buttons: list[InlineButton] | None = None,
             body: str | None = None,
             footer: str | None = None,
     ) -> str:
         """
         Send a document to a WhatsApp user.
 
         Example:
 
             >>> wa.send_document(
             ...     to="1234567890",
             ...     document="https://example.com/example_123.pdf",
-            ...     filename="Example PDF",
+            ...     file_name="exmaple.pdf",
             ...     caption="Example PDF"
             ... )
 
 
         Args:
             to: The phone ID of the WhatsApp user.
-            document: The document to send (either a URL or a file ID).
-            filename: The filename of the document (optional, The extension of the filename will specify what format the document is displayed as in WhatsApp).
+            document: The document to send (either a media ID, URL, file path, bytes, or a open file object).
+            file_name: The filename of the document (optional, The extension of the filename will specify what format the document is displayed as in WhatsApp).
             caption: The caption of the document (optional).
             reply_to_message_id: The message ID to reply to (optional).
             buttons: The buttons to send with the document (optional).
             body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).
             footer: The footer of the message (if buttons is provided, optional, markdown has no effect).
 
         Returns:
             The message ID of the sent message.
         """
+        is_url, document = self._resolve_media_param(media=document, mime_type="text/plain",
+                                                     file_name=file_name or "file.text")
         if not buttons:
             return self.api.send_media(
                 to=to,
                 media_id_or_url=document,
                 media_type="document",
                 reply_to_message_id=reply_to_message_id,
-                filename=filename,
+                file_name=file_name,
                 caption=caption,
             )['messages'][0]['id']
         if not body and not caption:
             raise ValueError("Either body or caption must be provided when sending a document with buttons.")
         return self.api.send_interactive_message(
             to=to,
             keyboard=buttons,
             header={
                 "type": "document",
                 "document": {
-                    "link" if document.startswith(("https://", "http://")) else "id": document,
-                    "filename": filename,
+                    "link" if is_url else "id": document,
+                    "filename": file_name,
                 }
             },
             body=body or caption,
             footer=footer,
             reply_to_message_id=reply_to_message_id,
         )['messages'][0]['id']
 
     def send_audio(
             self,
             to: str,
-            audio: str | bytes,
+            audio: str | bytes | BinaryIO,
             reply_to_message_id: str | None = None,
     ) -> str:
         """
         Send an audio file to a WhatsApp user.
 
         Example:
 
             >>> wa.send_audio(
             ...     to='1234567890',
             ...     audio='https://example.com/audio.mp3',
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
-            audio: The audio file to send (either a URL or a file ID).
+            audio: The audio file to send (either a media ID, URL, file path, bytes, or a open file object).
             reply_to_message_id: The message ID to reply to (optional).
 
         Returns:
             The message ID of the sent message.
         """
+        _, audio = self._resolve_media_param(media=audio, mime_type="audio/mpeg", file_name="audio.mp3")
         return self.api.send_media(
             to=to,
             media_id_or_url=audio,
             media_type="audio",
             reply_to_message_id=reply_to_message_id,
         )['messages'][0]['id']
 
     def send_sticker(
             self,
             to: str,
-            sticker: str | bytes,
+            sticker: str | bytes | BinaryIO,
             reply_to_message_id: str | None = None,
     ) -> str:
         """
         Send a sticker to a WhatsApp user.
             - A static sticker needs to be 512x512 pixels and cannot exceed 100 KB.
             - An animated sticker must be 512x512 pixels and cannot exceed 500 KB.
 
@@ -502,20 +532,21 @@
             >>> wa.send_sticker(
             ...     to='1234567890',
             ...     sticker='https://example.com/sticker.webp',
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
-            sticker: The sticker to send (either a URL or a file ID).
+            sticker: The sticker to send (either a media ID, URL, file path, bytes, or a open file object).
             reply_to_message_id: The message ID to reply to (optional).
 
         Returns:
             The message ID of the sent message.
         """
+        _, sticker = self._resolve_media_param(media=sticker, mime_type="image/webp", file_name="sticker.webp")
         return self.api.send_media(
             to=to,
             media_id_or_url=sticker,
             media_type="sticker",
             reply_to_message_id=reply_to_message_id,
         )['messages'][0]['id']
 
@@ -656,50 +687,66 @@
         Returns:
             Whether the message was marked as read.
         """
         return self.api.mark_message_as_read(message_id=message_id)['success']
 
     def upload_media(
             self,
-            media: str | bytes,
-            mime_type: str | None = None,
+            media: str | bytes | BinaryIO,
+            mime_type: str,
+            file_name: str | None = None,
     ) -> str:
         """
         Upload media to WhatsApp servers.
 
         Example:
             >>> wa.upload_media(
             ...     media='https://example.com/image.jpg',
             ...     mime_type='image/jpeg',
             ... )
 
         Args:
-            media: The media to upload (either a URL or a file Path or bytes).
-            mime_type: The MIME type of the media (optional).
+            media: The media to upload (can be a URL, bytes, or a file path).
+            mime_type: The MIME type of the media (required if media is bytes or a file path).
+            file_name: The file name of the media (optional).
 
         Returns:
             The media ID.
-
-        Raises:
-            ValueError: If mime_type is not provided and cannot be guessed (e.g. for bytes or URLs without
-                Content-Type header).
         """
+        if isinstance(media, str):
+            if os.path.isfile(media):
+                file, file_name, mime_type = \
+                    open(media, 'rb'), os.path.basename(media), (mimetypes.guess_type(media)[0] or mime_type)
+            elif media.startswith(("https://", "http://")):
+                res = requests.get(media)
+                res.raise_for_status()
+                file, file_name, mime_type = \
+                    res.content, os.path.basename(media) or file_name, (res.headers['Content-Type'] or mime_type)
+            else:
+                raise ValueError(f'File not found or invalid URL: {media}')
+        else:
+            file = media
         return self.api.upload_media(
-            media=media,
+            file_name=file_name or 'file',
+            media=file,
             mime_type=mime_type,
         )['id']
 
     def get_media_url(
             self,
             media_id: str
     ) -> MediaUrlResponse:
         """
         Get the URL of a media.
             - The URL is valid for 5 minutes.
-            - You can download with ``wa.download_media``.
+            - The media can be downloaded using the ``download`` method.
+
+        Example:
+            >>> wa.get_media_url(
+            ...
 
         Args:
             media_id: The media ID.
 
         Returns:
             A MediaResponse object with the media URL.
         """
@@ -713,34 +760,34 @@
             file_size=res['file_size'],
         )
 
     def download_media(
             self,
             url: str,
             path: str | None = None,
-            filename: str | None = None,
+            file_name: str | None = None,
             in_memory: bool = False,
     ) -> str | bytes:
         """
         Download a media file from WhatsApp servers.
 
         Args:
             url: The URL of the media file (from ``get_media_url``).
             path: The path where to save the file (if not provided, the current working directory will be used).
-            filename: The name of the file (if not provided, it will be guessed from the URL + extension).
+            file_name: The name of the file (if not provided, it will be guessed from the URL + extension).
             in_memory: Whether to return the file as bytes instead of saving it to disk (default: False).
 
         Returns:
             The path of the saved file if ``in_memory`` is False, the file as bytes otherwise.
         """
         content, mimetype = self.api.get_media_bytes(media_url=url)
         if in_memory:
             return content
         if path is None:
             path = os.getcwd()
-        if filename is None:
-            filename = hashlib.sha256(url.encode()).hexdigest() +\
-                       mimetypes.guess_extension(mimetype or 'application/octet-stream')
-        path = os.path.join(path, filename)
+        if file_name is None:
+            file_name = hashlib.sha256(url.encode()).hexdigest() + \
+                        mimetypes.guess_extension(mimetype) or '.bin'
+        path = os.path.join(path, file_name)
         with open(path, "wb") as f:
             f.write(content)
         return path
```

## pywa/filters.py

```diff
@@ -2,16 +2,18 @@
 from __future__ import annotations
 
 __all__ = (
     "all_",
     "any_",
     "not_",
     "FORWARDED",
+    "FORWARDED_MANY_TIMES",
     "from_user",
     "TextFilter",
+    "MediaFilter",
     "ImageFilter",
     "VideoFilter",
     "AudioFilter",
     "DocumentFilter",
     "StickerFilter",
     "ReactionFilter",
     "UnsupportedMsgFilter",
@@ -41,14 +43,21 @@
 FORWARDED: MessageT = lambda wa, m: m.forwarded
 """
 Filter for forwarded messages.
 
 >>> filters.FORWARDED
 """
 
+FORWARDED_MANY_TIMES: MessageT = lambda wa, m: m.forwarded_many_times
+"""
+Filter for messages that have been forwarded many times.
+
+>>> filters.FORWARDED_MANY_TIMES
+"""
+
 
 def all_(*filters: Callable[[Wa, T], bool]) -> Callable[[Wa, T], bool]:
     """
     Filter for messages that pass all the given filters.
 
     >>> all_(TextFilter.startswith("World"), TextFilter.contains("Word"))
     """
@@ -87,23 +96,36 @@
 
 from_users = from_user  # alias
 from_number = from_user  # alias
 from_numbers = from_user  # alias
 
 
 class _BaseUpdateFilter:
-
+    """
+    Base class for all filters.
+    """
     __message_types__: tuple[Mt, ...] = ()
     
     @classmethod
     def _match_type(cls, m: Msg) -> bool:
         return m.type in cls.__message_types__
 
 
-class _MediaFilter(_BaseUpdateFilter):
+class MediaFilter(_BaseUpdateFilter):
+    """
+    Useful filters for media messages.
+    """
+    __message_types__ = (Mt.IMAGE, Mt.VIDEO, Mt.AUDIO, Mt.DOCUMENT, Mt.STICKER)
+
+    ANY: MessageT = lambda wa, m: m.has_media
+    """
+    Filter for all media messages.
+    
+    >>> MediaFilter.ANY
+    """
 
     @classmethod
     def mimetype(cls, *mimetypes: str) -> MessageT:
         """
         Filter for media messages that match any of the given mime types.
             - Aliases: ``mimetypes``, ``mime_type``, ``mime_types``
             - See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
@@ -115,15 +137,15 @@
         )
 
     mimetypes = mimetype  # alias
     mime_type = mimetype  # alias
     mime_types = mimetype  # alias
 
 
-class _MediaWithCaptionFilter(_MediaFilter):
+class _MediaWithCaptionFilter(MediaFilter):
     @classmethod
     def _has_caption(cls, wa: Wa, m: Msg) -> bool:
         return cls._match_type(m) and m.caption is not None
 
     HAS_CAPTION: MessageT = _has_caption
     """
     Filter for media messages that have a caption.
@@ -309,15 +331,15 @@
     """
     Filter for all document messages.
     
     >>> DocumentFilter.ANY
     """
 
 
-class AudioFilter(_MediaFilter):
+class AudioFilter(MediaFilter):
     """Useful filters for audio messages."""
 
     __message_types__ = (Mt.AUDIO,)
 
     ANY: MessageT = lambda wa, m: AudioFilter._match_type(m)
     """
     Filter for all audio messages (voice notes and audio files).
@@ -336,15 +358,15 @@
     """
     Filter for audio messages that are audio files.
     
     >>> AudioFilter.AUDIO
     """
 
 
-class StickerFilter(_MediaFilter):
+class StickerFilter(MediaFilter):
     """Useful filters for sticker messages."""
 
     __message_types__ = (Mt.STICKER,)
 
     ANY: MessageT = lambda wa, m: StickerFilter._match_type(m)
     """
     Filter for all sticker messages.
```

## pywa/utils.py

```diff
@@ -1,13 +1,8 @@
-import math
 from importlib import import_module
-from typing import Callable, TYPE_CHECKING
-if TYPE_CHECKING:
-    from pywa import WhatsApp
-    from pywa.types import MessageType, Message
 
 
 def is_fastapi_app(app):
     """Check if the app is a FastAPI app."""
     try:
         return isinstance(app, import_module("fastapi").FastAPI)
     except ImportError:
@@ -22,13 +17,14 @@
         return False
 
 
 def get_distance(lat1: float, lon1: float, lat2: float, lon2: float) -> float:
     """
     Calculate the distance between two points on Earth using the Haversine formula.
     """
+    math = import_module("math")
     lon1, lat1, lon2, lat2 = map(math.radians, [lon1, lat1, lon2, lat2])
     return (2 * math.asin(
         math.sqrt(
             math.sin((lat2 - lat1) / 2) ** 2 + math.cos(lat1) * math.cos(lat2) * math.sin((lon2 - lon1) / 2) ** 2)
     )) * 6371
```

## pywa/webhook.py

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 """The webhook module contains the Webhook class, which is used to register a webhook to listen for incoming 
 messages."""
 
 import collections
+import threading
 from typing import Union, TYPE_CHECKING, Callable, Any
-from pywa.types import Message, CallbackButton, CallbackSelection, MessageStatus, BaseUpdate
+from pywa.types import Message, CallbackButton, CallbackSelection, MessageStatus
+from pywa.types.base_update import BaseUpdate
 from pywa import utils
 
 if TYPE_CHECKING:
     from pywa import WhatsApp
 
 __all__ = ["Webhook"]
 
@@ -28,62 +30,63 @@
         self.handlers: dict[str, list[Callable[[WhatsApp, BaseUpdate | dict], Any]]] = collections.defaultdict(list)
         self.wa_client = wa_client
         self.server = server
         self.verify_token = verify_token
         self.webhook_endpoint = webhook_endpoint
         self.filter_updates = filter_updates
 
+        hub_vt = "hub.verify_token"
+        hub_ch = "hub.challenge"
+
         if utils.is_flask_app(self.server):
             import flask
 
-            @self.server.before_request
-            def before_request():
-                if flask.request.path != self.webhook_endpoint:
-                    return
-                if flask.request.method == "GET":
-                    if flask.request.args.get("hub.verify_token") == self.verify_token:
-                        return flask.request.args.get("hub.challenge"), 200
-                    else:
-                        return "Error, invalid verification token", 403
-                elif flask.request.method == "POST":
-                    self.call_handlers(update=flask.request.json)
-                    return "ok", 200
+            @self.server.route(self.webhook_endpoint, methods=["GET"])
+            def verify_token():
+                if flask.request.args.get(hub_vt) == self.verify_token:
+                    return flask.request.args.get(hub_ch), 200
+                return "Error, invalid verification token", 403
+
+            @self.server.route(self.webhook_endpoint, methods=["POST"])
+            def webhook():
+                threading.Thread(target=self.call_handlers, args=(flask.request.json,)).start()
+                return "ok", 200
 
         elif utils.is_fastapi_app(self.server):
             import fastapi
 
-            @self.server.middleware("http")
-            async def before_request(request: fastapi.Request, call_next: Callable):
-                if request.url.path != self.webhook_endpoint:
-                    return await call_next(request)
-                if request.method == "GET":
-                    if request.query_params.get("hub.verify_token") == self.verify_token:
-                        return fastapi.Response(content=request.query_params.get("hub.challenge"), status_code=200)
-                    else:
-                        return fastapi.Response(content="Error, invalid verification token", status_code=403)
-                elif request.method == "POST":
-                    request_body = await request.json()
-                    self.call_handlers(update=request_body)
-                    return fastapi.Response(content="ok", status_code=200)
-                return await call_next(request)
+            @self.server.get(self.webhook_endpoint)
+            def verify_token(
+                    token: str = fastapi.Query(..., alias=hub_vt),
+                    challenge: str = fastapi.Query(..., alias=hub_ch)
+            ):
+                if token == self.verify_token:
+                    return fastapi.Response(content=challenge, status_code=200)
+                return fastapi.Response(content="Error, invalid verification token", status_code=403)
+
+            @self.server.post(self.webhook_endpoint)
+            def webhook(payload: dict = fastapi.Body(...)):
+                threading.Thread(target=self.call_handlers, args=(payload,)).start()
+                return fastapi.Response(content="ok", status_code=200)
 
         else:
-            raise ValueError("The app must be a Flask or FastAPI app.")
+            raise ValueError("The server must be a Flask or FastAPI app.")
 
     def call_handlers(self, update: dict) -> None:
         """Call the handlers for the given update."""
         try:
             if not self.filter_updates or (
-                    update["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"] == self.wa_client.phone_id):
+                    update["entry"][0]["changes"][0]["value"]["metadata"][
+                        "phone_number_id"] == self.wa_client.phone_id):
                 for raw_update_handler in self.handlers["raw_update"]:
                     raw_update_handler(self.wa_client, update)
                 update, key = self.convert_dict_to_update(client=self.wa_client, d=update)
                 if key is None:
                     return
-                for handler in self.handlers[key]:  # TODO execute in parallel
+                for handler in self.handlers[key]:
                     handler(self.wa_client, update)
         except (KeyError, IndexError):  # the update not send to this phone and filter_updates is True
             pass
 
     @staticmethod
     def convert_dict_to_update(client: WhatsApp, d: dict) -> tuple[BaseUpdate | None, str | None]:
         """Convert a webhook dict to a BaseUpdate object."""
@@ -96,8 +99,7 @@
                     return CallbackButton.from_dict(client=client, value=value), "button"
                 elif value["messages"][0]["interactive"]["type"] == "list_reply":
                     return CallbackSelection.from_dict(client=client, value=value), "selection"
 
         elif 'statuses' in value:
             return MessageStatus.from_dict(client=client, value=value), "message_status"
         return None, None  # the update is not supported
-
```

## Comparing `pywa-0.0.1rc16.dist-info/LICENSE` & `pywa-0.0.1rc17.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc16.dist-info/METADATA` & `pywa-0.0.1rc17.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc16
+Version: 0.0.1rc17
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
@@ -19,14 +19,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: requests-toolbelt
 Provides-Extra: fastapi
 Requires-Dist: fastapi ; extra == 'fastapi'
 Requires-Dist: uvicorn ; extra == 'fastapi'
 Provides-Extra: flask
 Requires-Dist: flask ; extra == 'flask'
 
 .. image:: https://i.imgur.com/hbGP0rW.png
```

## Comparing `pywa-0.0.1rc16.dist-info/RECORD` & `pywa-0.0.1rc17.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 pywa/__init__.py,sha256=u98CpT0wYk8-XDPUGB_hW-a_23agBkzTSzfwmoqnsE0,117
-pywa/__version__.py,sha256=M93UajZ2PPnX4gqdGnY2tyhRbdEJ1BncArFGCRSHvkM,26
-pywa/api.py,sha256=G3NL2PKhGO7YhrVeEz2bfJhGNfD7j1lGwgKnhsZpAuU,14991
-pywa/client.py,sha256=ita4mY7UfM8xwjvEV_a60-3W4frC3uAJP-xumP5oYdM,26847
+pywa/__version__.py,sha256=DlFrhUG4bi9E-87CieAzje8rjSKLjHTgQ3wNJ8fl9T8,26
+pywa/api.py,sha256=rx6ceDInJ_1srH65PNNub7CYwb9BHM7_dXAuC0OF9FQ,14468
+pywa/client.py,sha256=3ioAyAwVD320CPbEJP07kfkGzog4JEXTB0Gge3cbF_A,29314
 pywa/errors.py,sha256=ErB0UGIpIOF5vZXK39WmiSrB_PSYvTJL8PLIp90vTjU,7191
-pywa/filters.py,sha256=2-hPWfevDpLsnJIvdsXdkRvazJyKGNsxHIAalJ6i48w,20703
+pywa/filters.py,sha256=Iqcah-FLKkAbeKdSHEm33bGOPe-2E-eDa7-1DrXFKnc,21225
 pywa/handlers.py,sha256=DTlKr-yvVKpTgh3F0Gsq78gT5XhBIo_VVnYHz3lu25w,1794
-pywa/types.py,sha256=PKCefN4pMLNn9Dx_fbBXEUohGFEhMeGLTZfW-F4gYBU,39628
-pywa/utils.py,sha256=GRTfSvmsuOBd1_Yw2c90XoALqVPuy6HzyvJuqg3xjtI,991
-pywa/webhook.py,sha256=UFsV3UyltYLj3MYjURG6YImjU4hYVHkDffweyEe1Jdc,4613
-pywa-0.0.1rc16.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc16.dist-info/METADATA,sha256=eOdVyuz_KnoR9ZRFIyCobhAERtFK4x87soHl_5YYWoA,4387
-pywa-0.0.1rc16.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc16.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc16.dist-info/RECORD,,
+pywa/utils.py,sha256=vIPGDuXFo80xAhv88mboE-rU-uDEv594cAxEPsMrIZg,873
+pywa/webhook.py,sha256=XJEJRKLk8Dg4eJ1qE5_B3bUXu0ugt-0cjWe8C9tbvH4,4449
+pywa/types/__init__.py,sha256=HwhabvWT9b1bgPLnvXBDOmYNTh-FYjCC-ot-rh8xqzo,336
+pywa/types/base_update.py,sha256=Jd3JW8nhFd2ss0ftBjr8mEKw1gVhxlOcbKosPdQwPhA,9301
+pywa/types/callback.py,sha256=J7xDPPeGaU_JPpbdyJXJtmVu7hTMMlyquqQI9p95F5w,5653
+pywa/types/media.py,sha256=4T5yOsoZwFmJaTUZf49VnMsXACsGLq1crC6wzSBqanA,4609
+pywa/types/message.py,sha256=zNKvifHA3P89TOxKoV4dLnt-B9jbu7whlP8gdu304Xo,11234
+pywa/types/message_status.py,sha256=wgUlrgTCaKKqEZgVaZt_yYY_PKyJMhBGz-Rh3WaXSB0,1934
+pywa/types/others.py,sha256=UeXSWEY1pekZDVBDacbUsXff_OmYbxbAe9P2o_am4es,9156
+pywa-0.0.1rc17.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc17.dist-info/METADATA,sha256=ncFGGg_nCInvGdfHKC5lUpY2DXkz9m3bG3SZ9fRaluo,4420
+pywa-0.0.1rc17.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc17.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc17.dist-info/RECORD,,
```

