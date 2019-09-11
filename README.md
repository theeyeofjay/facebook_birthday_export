Facebook Birthday Export
===

Facebook has recently removed the feature to download the birthday calendar.

This script will allow you to get all the birthdays in a CSV format (with some manual efforts) which you can the easily import to Google Calendar.

You can also visit [https://deepakmahakale.in/facebook_birthday_export](https://deepakmahakale.in/facebook_birthday_export)

## Update: Chrome extension is now available

[Facebook Birthdays Export](https://chrome.google.com/webstore/detail/facebook-birthdays-export/hhbdbekeaphpjhoadmgibhdbfehnmpdc)

## Steps

1. Login to Facebook
2. Visit [Facebook's events page](https://www.facebook.com/events/birthdays)
3. Scroll to the bottom of the page till you have birthdays from all the months
4. Right click on **Today's Birthday** or **Upcoming Birthdays**
5. Select **Inspect** from the dropdown
6. In html inspector right click on div with `id="birthdays_content"` and select "copy" > "Copy element"
  ![facebook_inspect](https://user-images.githubusercontent.com/14993828/63705538-009e7d80-c84b-11e9-9f13-5c8da95996a0.png)

8. Paste the content in `facebook_html.txt` and run the following command
    ```shell
    python birthday_parser.py
    ```
9. Import the **birthdays.csv** generated by the program to Google Calendar

### References:

[CSV Format for Google Calendar](https://support.google.com/calendar/answer/37118?hl=en)
