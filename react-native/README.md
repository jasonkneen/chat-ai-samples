# [React Native](https://getstream.io/blog/react-native-assistant/) AI components Sample App

This repository contains a sample AI assistant app that integrates Stream's [React Native Chat SDK](https://github.com/GetStream/stream-chat-react-native). The sample shows how to render responses from LLM providers such as ChatGPT, Gemini, Anthropic or any custom backend by using our AI components and server-side SDKs. Our UI components are able to render Markdown, Code blocks, tables, thinking indicators, images, etc.

The sample shows you how to integrate the following views:
- `StreamingMessageView` - a component that is able to render text, markdown and code in real-time, using character-by-character animation, similar to ChatGPT (and is available by default !).
- `AITypingIndicatorView` - a component that can display different states of the LLM (thinking, checking external sources, etc).
- `StopMessageStreamingButton` - a component that replaces the `SendMessage` button by default and adds a way to stop AI generation

These components are designed to work seamlessly with our existing React Native SDK UI [Chat SDK](https://getstream.io/chat/docs/sdk/react-native/ui-components/overview/). Our [developer guide](https://getstream.io/chat/solutions/ai-integration/) explains how to get started building AI integrations with Stream and React Native.

The app consists of the standard StreamChat `ChannelList` and `Channel` screens. The channel view is enhanced with a button to start and stop AI agents. When the agent is started, it listens to all the sent messages in the channel and connects to an LLM to receive AI-generated responses.

There's also an example that shows you how to present the different states of the LLM, by reacting to the new AI events in the SDK. Additionally, you will learn how to stop the generation of messages at any time, using the `StopMessageStreamingButton`.

## ⚙️ Usage

Running the app is simple. All you need to do is open the project in your favourite IDE, run the required installations:

```bash
yarn install
npx pod-install
```
and then run the app in your desired environment:

```bash
yarn start --reset-cache # to run Metro
yarn ios # for iOS
yarn android # for Android
```

If you want to use your own server, make sure to update the `url` parameters in `./http/requests.ts` to your own server's.

<br />

<a href="https://getstream.io?utm_source=Github&utm_medium=Github_Repo_Content&utm_content=Developer&utm_campaign=Github_Swift_AI_SDK&utm_term=DevRelOss">
<img src="https://user-images.githubusercontent.com/24237865/138428440-b92e5fb7-89f8-41aa-96b1-71a5486c5849.png" align="right" width="12%"/>
</a>

## 🛥 What is Stream?

Stream allows developers to rapidly deploy scalable feeds, chat messaging and video with an industry leading 99.999% uptime SLA guarantee.

Stream provides UI components and state handling that make it easy to build real-time chat and video calling for your app. Stream runs and maintains a global network of edge servers around the world, ensuring optimal latency and reliability regardless of where your users are located.

## 📕 Tutorials

To learn more about integrating AI and chatbots into your application, we recommend checking out the full list of tutorials across all of our supported frontend SDKs and providers. Stream's Chat SDK is natively supported across:
* [React](https://getstream.io/blog/react-assistant/)
* [React Native](https://getstream.io/blog/react-native-assistant/)
* [Jetpack Compose](https://getstream.io/blog/android-assistant/)
* [Swift UI](https://getstream.io/blog/ios-assistant/)
* [Flutter](https://getstream.io/blog/flutter-assistant/)


## 👩‍💻 Free for Makers 👨‍💻

Stream is free for most side and hobby projects. To qualify, your project/company needs to have < 5 team members and < $10k in monthly revenue. Makers get $100 in monthly credit for video for free.
For more details, check out the [Maker Account](https://getstream.io/maker-account?utm_source=Github&utm_medium=Github_Repo_Content&utm_content=Developer&utm_campaign=Github_Swift_AI_SDK&utm_term=DevRelOss).

## 💼 We are hiring!

We've recently closed a [\$38 million Series B funding round](https://techcrunch.com/2021/03/04/stream-raises-38m-as-its-chat-and-activity-feed-apis-power-communications-for-1b-users/) and we keep actively growing.
Our APIs are used by more than a billion end-users, and you'll have a chance to make a huge impact on the product within a team of the strongest engineers all over the world.
Check out our current openings and apply via [Stream's website](https://getstream.io/team/#jobs).


## License

```
Copyright (c) 2014-2024 Stream.io Inc. All rights reserved.

Licensed under the Stream License;
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   https://github.com/GetStream/stream-chat-swift-ai/blob/main/LICENSE

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
