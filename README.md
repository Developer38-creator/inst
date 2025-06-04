# website link-
https://developer38-creator.github.io/Video-player-inst/
# Instagram-like Video Feed
This HTML code creates a basic Instagram-like vertical video feed. It features:

-   **Vertical Scrolling:** Videos snap to the center of the viewport as you scroll.
-   **Video Playback:** Single tap on a video to play/pause. The first video autoplays.
-   **Double Tap Like:** Double tap on a video to show a heart animation, simulating a "like".
-   **Basic UI:** Includes a camera icon, like, comment, share, and three-dots icons, user profile information with a follow button, and a music icon.

## Technologies Used

-   HTML
-   Tailwind CSS (via CDN)
-   Font Awesome (via CDN)

## How to Use

1.  Save the provided HTML code as `index.html`.
2.  Create a folder named `Videos` in the same directory.
3.  Place your video files (named `7221400.mp4` in this example) inside the `Videos` folder. You'll need to update the `videos` array in the `<script>` section to point to your actual video file names.
4.  (Optional) Create a folder named `Images` and place thumbnail images (named `IMG-20250526-WA0003.jpg` in this example) inside. Update the `thumbnail` property in the `videos` array accordingly.
5.  Open `index.html` in your web browser.

## Structure

The HTML is structured as follows:

-   A main `div` with the ID `video-scroll` acts as the scrollable container. It uses Tailwind CSS classes for full-screen height, width, vertical overflow with snapping, and to hide the scrollbar.
-   JavaScript dynamically generates `div` elements for each video. Each video container includes:
    -   A `<video>` element to display the video.
    -   An overlay `div` for UI elements (icons, user info).
    -   A heart icon `i` element for the like animation.
-   Tailwind CSS classes are extensively used for styling.
-   Font Awesome icons are used for the UI elements.
-   JavaScript handles:
    -   Dynamically creating video elements based on the `videos` array.
    -   Playing/pausing videos on single tap.
    -   Showing the like animation on double tap.
    -   Autoplaying the first video.
    -   Pausing videos that are not fully in the viewport and playing the one that is.

## Customization

-   **Videos:** Modify the `videos` array in the `<script>` section to add or change the video sources, titles, and thumbnails. Ensure the file paths are correct.
-   **Styling:** You can further customize the appearance by modifying the inline `<style>` section or by adding more Tailwind CSS classes.
-   **Functionality:** The JavaScript can be extended to add more interactive features.

