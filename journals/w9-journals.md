# Weekly Project Journal --- PharmaFlow AI

**Project:** PharmaFlow AI --- AI-Powered Pharmacy Management System\
**Work Area:** Frontend, UI/UX Design, Documentation, and Voice
Assistant Integration\
**Journal Period:** Additional Week --- Voice-Based Record Lookup and
Catalogue Assistance

## 1. Objective for the Week

The objective for this week was to extend the PharmaFlow AI interface
with voice-and-chat functionality so that a user can search medicine
catalogue records more conveniently. The feature is intended to support
typed queries as well as microphone input and to present catalogue
information in a clear, user-friendly format.

## 2. Work Completed

### Voice Assistant Interface

-   Added/updated a **Voice Assistant** panel within the PharmaFlow AI
    interface.
-   Included a language selector, a **Read replies aloud** option, a
    **Clear chat** control, and a text input for entering a medicine
    name or query.
-   Added a **Start microphone** control to support voice-based input,
    along with a visible status message to guide the user.
-   Displayed user queries and assistant responses as separate chat
    messages to make the interaction easy to follow.

### Medicine Catalogue and Record Lookup

-   Added a conversational lookup flow for questions about medicine
    records, such as whether ORS powder appears in the catalogue.
-   The demonstrated query, "Is ORS powder in inventory?", returned a
    catalogue match for **ORS Powder 21.8 g**.
-   The response clearly distinguishes a catalogue match from confirmed
    stock availability or current pricing. It directs the user to verify
    stock and price at the pharmacy counter rather than presenting
    unverified information as fact.
-   Included quick-action controls such as **Catalogue report**, **Find
    Crocin**, and **Prescription help** to make common follow-up tasks
    easier to access.

### User Guidance and Safety

-   Included a note that catalogue assistance is not medical advice.
-   Added guidance to ask a pharmacist to confirm prescription
    requirements where relevant.
-   Included a reminder to review the speech transcript before sending
    it, helping reduce errors caused by speech recognition.
-   Kept the chat interaction on the current page, supporting a focused
    workflow.

## 3. Implementation and Design Considerations

-   Focused on a simple, accessible layout with clearly labelled
    controls and readable chat messages.
-   Designed the flow to support both keyboard-based queries and
    microphone-based input.
-   Used quick-action prompts to reduce the number of steps needed for
    common catalogue tasks.
-   Kept the response wording cautious: catalogue records can help
    locate a medicine entry, but they do not by themselves verify live
    inventory, price, or prescription eligibility.
-   The voice feature depends on browser microphone permissions and may
    use the browser's speech services, depending on the implementation
    and browser support.

## 4. Testing and Observations

The interface was reviewed using a sample query about ORS powder.

**Observed behaviour:** 1. The user entered a medicine availability
question. 2. The assistant displayed a matching catalogue entry: ORS
Powder 21.8 g. 3. The response explained that stock and price must be
checked separately. 4. Quick-action options were displayed for related
catalogue and help tasks. 5. The panel provided controls for microphone
input, spoken replies, clearing the conversation, and entering another
medicine name.

This check demonstrates the intended catalogue-lookup interaction. It
does **not** establish that live inventory integration, real-time
pricing, or every voice-browser combination has been fully tested.

## 5. Challenges and Considerations

-   A catalogue result must not be presented as proof that a medicine is
    currently in stock.
-   Speech recognition can misinterpret medicine names, quantities, and
    similar-sounding words; the transcript should be reviewed before
    submission.
-   Microphone access and spoken-reply support can vary by browser and
    permission settings.
-   Medical and prescription-related responses must remain informational
    and should direct users to a pharmacist when confirmation is
    required.

## 6. Outcome of the Week

The project interface now demonstrates an additional voice-and-chat
workflow for searching medicine catalogue records. It combines text
entry, microphone input controls, optional spoken replies, contextual
quick actions, and cautious messaging about inventory and prescription
confirmation. This improves the usability of the pharmacy interface and
provides a foundation for further integration with verified backend
records.

## 7. Next Steps

-   Connect catalogue queries to the appropriate backend/database
    records and validate the returned fields.
-   If live inventory is required, retrieve stock quantities from the
    inventory system rather than inferring availability from catalogue
    entries.
-   Add appropriate loading, empty-result, and error states for failed
    or unmatched queries.
-   Test voice input with common medicine names and review recognition
    accuracy.
-   Verify microphone permissions and read-aloud behaviour across
    supported browsers.
-   Update project screenshots and documentation after the integration
    and testing are complete.

## 8. Learning and Contribution

This week's work focused on improving the pharmacy system's user
interaction through voice-and-chat controls and record lookup. It also
reinforced the importance of separating catalogue information from live
operational data, presenting clear user guidance, and documenting the
limits of a feature instead of claiming unverified functionality.
