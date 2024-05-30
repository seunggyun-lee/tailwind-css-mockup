https://chatgpt.com/share/9f5ed2d3-092a-4933-bf9d-47895e126318

you are tailwind html developer now.
I'll make infobox component.

- use tailwind css, avoid style attribute
- color css -> use tailwind.config

  - `--grayishblue_300: #DFE6F1`
  - `--grayishblue_200: #EDF2FA`
  - `--grayishblue_100: #F6FAFF`
  - `--grayishblue_600: #9BA7BA`
  - `--brand_black_1000: #525252`

- container

  - flex display
  - 2 sections
  - border-radius: 12px;
  - `border: 1px solid var(--grayishblue_300)`
  - padding: 0;

  - first section

    - width: 64px;
    - flex display
    - center align
    - `background-color: var(--grayishblue_200)`
    - has svg
      ```
      <svg width="32" height="32" viewBox="0 0 16 16" fill="var(--grayishblue_600)" xmlns="http://www.w3.org/2000/svg" style="color: var(--grayishblue_600);"><path d="M8 14.35C11.507 14.35 14.35 11.507 14.35 8.00002C14.35 4.49302 11.507 1.65002 8 1.65002C4.49299 1.65002 1.65 4.49302 1.65 8.00002C1.65 11.507 4.49299 14.35 8 14.35ZM8.75 6.74579C8.75 7.16 8.41421 7.49579 8 7.49579L7.5 7.49597V9.16577H8.5V8.42332C9.22287 8.20818 9.75 7.53854 9.75 6.74579C9.75 5.77929 8.9665 4.99579 8 4.99579C7.0335 4.99579 6.25 5.77929 6.25 6.74579H7.25C7.25 6.33157 7.58579 5.99579 8 5.99579C8.41421 5.99579 8.75 6.33157 8.75 6.74579ZM8 11.0037C8.34242 11.0037 8.62 10.7261 8.62 10.3837C8.62 10.0413 8.34242 9.76373 8 9.76373C7.65759 9.76373 7.38 10.0413 7.38 10.3837C7.38 10.7261 7.65759 11.0037 8 11.0037Z" fill-rule="evenodd" clip-rule="evenodd" fill="currentColor" opacity="1"></path></svg>
      ```

  - second section
    - flex display
    - space-between center align
    - padding: 18px 20px;
    - `background-color: var(--grayishblue_100)`
    - 2 sections
    - left section
      - text: `카카오톡 채널 친구인 고객에게 카카오톡으로 타겟팅 메시지를 발송해 구매전환율을 높이는 캠페인입니다.`
      - font-size: 14px;
    - right section
      - gap: 2px
      - svg
        ```
        <svg width="14" height="14" viewBox="0 0 16 16" fill="var(--brand_black_1000)" xmlns="http://www.w3.org/2000/svg" style="color: var(--brand_black_1000);"><path d="M13.35 8.00002C13.35 10.9547 10.9547 13.35 8 13.35C5.04528 13.35 2.65 10.9547 2.65 8.00002C2.65 5.0453 5.04528 2.65002 8 2.65002C10.9547 2.65002 13.35 5.0453 13.35 8.00002ZM14.35 8.00002C14.35 11.507 11.507 14.35 8 14.35C4.49299 14.35 1.65 11.507 1.65 8.00002C1.65 4.49302 4.49299 1.65002 8 1.65002C11.507 1.65002 14.35 4.49302 14.35 8.00002ZM8 7.49579C8.41421 7.49579 8.75 7.16 8.75 6.74579C8.75 6.33157 8.41421 5.99579 8 5.99579C7.58579 5.99579 7.25 6.33157 7.25 6.74579H6.25C6.25 5.77929 7.0335 4.99579 8 4.99579C8.9665 4.99579 9.75 5.77929 9.75 6.74579C9.75 7.53854 9.22287 8.20818 8.5 8.42332V9.16577H7.5V7.49597L8 7.49579ZM8.62 10.3837C8.62 10.7261 8.34242 11.0037 8 11.0037C7.65759 11.0037 7.38 10.7261 7.38 10.3837C7.38 10.0413 7.65759 9.76373 8 9.76373C8.34242 9.76373 8.62 10.0413 8.62 10.3837Z" fill-rule="evenodd" clip-rule="evenodd" fill="currentColor" opacity="1"></path></svg>
        ```
      - text: `구매전환율이란?`
        - font-size: 12px;
      - hover tooltip
        - text: `메시지를 받고 24시간 이내에 방문한 고객이 24시간 이내에 구매한 고객수 / 발송수입니다.`
        - background-color: black
        - location: left of svg
