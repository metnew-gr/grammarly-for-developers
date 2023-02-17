# Grammarly Text Editor SDK with Session and Document Stats

This demo shows how to track session and [document](https://developer.grammarly.com/docs/api/editor-sdk/documentstats) stats using the Grammarly Text Editor Plugin's built-in [callback functions](https://developer.grammarly.com/docs/api/editor-sdk/grammarlyeditorplugincallbacks#ondocumentstats).

[`SessionStats`](https://developer.grammarly.com/docs/api/editor-sdk/sessionstats) is an event that contains statistics about the [user's] Grammarly session, whereas [`DocumentStats`](https://developer.grammarly.com/docs/api/editor-sdk/documentstats) is an event that contains statistics about the user-entered text.

**Note**: The ability to receive real-time session and document stats is only available on the [Plus plan](https://developer.grammarly.com/plans).

## Try the demo

You can try the demo in [CodeSandbox](https://codesandbox.io/s/github/grammarly/grammarly-for-developers/tree/main/examples/editor-sdk-react-stats?file=/src/Editor.js).

## How it works

The `GrammarlyEditorPlugin` exposes the [`onSessionStats`](https://developer.grammarly.com/docs/api/editor-sdk/grammarlyeditorplugincallbacks#onsessionstats) and [`onDocumentStats`](https://developer.grammarly.com/docs/api/editor-sdk/grammarlyeditorplugincallbacks#ondocumentstats) properties. The `onSessionStats` callback executes with a [`SessionStats`](https://developer.grammarly.com/docs/api/editor-sdk/sessionstats) event triggered when new session information is available. The `onDocumentStats` callback executes with a [`DocumentStats`](https://developer.grammarly.com/docs/api/editor-sdk/documentstats) event when text is written.

## Get the code

A copy of this code is available in the [Grammarly for Developers GitHub repo](https://github.com/grammarly/grammarly-for-developers/tree/main/examples/editor-sdk-react-stats).

## Ask a question

If you want to ask a question, share a suggestion, or chat about how you're using the Grammarly Text Editor SDK in your application, join us in the [Grammarly for Developers Discussions](https://github.com/grammarly/grammarly-for-developers/discussions).
