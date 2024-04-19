# Logging into the training account

## Step 1
In a private browser window, use the following credentials to log into New Relic: 

- URL: [https://one.newrelic.com/](https://one.newrelic.com/)
- Email: demotron@newrelicuniversity.com
- Password: o11y-as-code

## Step 2
![](/images/other-users.jpg)

Select the user name in the lower left corner, then select _Other Users_. Confirm that _Demogorgon - Default_ is the current (grayed-out) organization. If it is not, select that organization and log in again when prompted.

# _Lab:_ Explore an APM service

Select the **Currency Service** in the **Demogorgon Prod** account. Set the time picker to 24 hours, then use the _Summary_ page to answer the following questions:

1. Is this service susceptible to any known security vulnerabilities? How do you know?

2. _True or False:_ This service contributes to more than 50% of the time it takes for the application to process a web transaction.

3. What is the meaning of the grey vertical “lollipops” that appear on several charts? Which summary tile shows data related to these markers?

4. Which of the following key performance indicators (KPIs) appear on the _Summary_ page? 

    a. Page view time

    b. Response time

    c. Database backup frequency

    d. Error rate

    e. Error user impact

    f. Throughput

    g. Account license key

5. Examine an alert issue (open or closed) associated with this service. If you were on an engineer on the team responsible for this application, how would you use the issue data?

## Additional resources
[New Relic documentation: _Troubleshoot with the APM summary page_](https://docs.newrelic.com/docs/apm/agents/manage-apm-agents/agent-data/triage-run-diagnostics/)

# _Lab:_ Managing agent data

Select the **Frontend** service in the **Demogorgon Prod** account. Set the time picker to 24 hours, then use the _Summary_ page to answer the following questions:

1. _Yes or No:_ Because this service appears in New Relic under _Services - APM_ we know that it is instrumented with an APM agent, but is its underlying infrastucture instrumented with New Relic Infrastructure?

2. On how many instances (hosts or containers) is this service hosted?

3. How can you see the logs for only this service? How can you further filter the logs to show only those with a level of _warning_ or _error_?

4. Find a distributed trace for this service. Are there logs associated with the trace? If so, how can you view them?

5. Select _Query Your Data_ from New Relic&rsquo;s main menu. Use the Data Explorer to create a query that augments technical data for the Frontend service with business data, to understand and visualize how this service is performing against key business metrics. Post your query in Zoom chat.

## Additional resources
- [Distributed tracing documentation](https://docs.newrelic.com/docs/distributed-tracing/concepts/introduction-distributed-tracing/)
- [Data explorer documentation](https://docs.newrelic.com/docs/query-your-data/explore-query-data/browse-data/introduction-data-explorer/#explore-data)

# _Lab:_ Visualizing insights

Select the **Checkout Service** in the **Demogorgon Prod** account. Set the time picker to 24 hours and answer the following questions:

1. View the underlying queries for several of the charts on the _Summary_ page. What do most of them have in common? Can you find any whose queries are unusual?

2. How are the transactions in the Transactions table sorted by default?

3. In the _Infrastructure_ section, use the dropdown menus to view the available options for each chart. Where does the data for each option come from?

4. Select _Service Levels_ from New Relic&rsquo;s main menu. Locate a service level that is out of compliance. If this were your account, what next step(s) would you recommend?

## Additional resources
[New Relic documentation: _Get started with New Relic service levels_](https://docs.newrelic.com/docs/service-level-management/intro-slm/)

# _Lab:_ Full stack observability practices

Select the **Checkout Service** in the **Demogorgon Prod** account. Set the time picker to 24 hours and answer the following questions:

1. Were there any **expected** errors during the selected time period? What determines whether expected errors are shown on the _Errors_ page?

2. On the _Errors_ page, what does the _Occurences_ column show?

3. Select the _Last deployment_ tile on the _Summary_ page. What can you learn about how the last deployment affected the service&rsquo;s performance? How did the deployment affect the Apdex score?

4. _Bonus:_ Using your personal New Relic account, use the [NerdGraph API Explorer](https://docs.newrelic.com/docs/apis/nerdgraph/get-started/nerdgraph-explorer/) to create a change marker for a simulated deployment.

## Additional resources
- [Errors inbox documentation](https://docs.newrelic.com/docs/errors-inbox/errors-inbox/)
- [NerdGraph API Explorer tutorial](https://docs.newrelic.com/docs/apis/nerdgraph/get-started/nerdgraph-explorer/)
- [Change tracking documentation](https://docs.newrelic.com/docs/change-tracking/change-tracking-introduction/)
