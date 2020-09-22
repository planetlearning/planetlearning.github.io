<div id="paypal-button-container"></div>
<script src="https://www.paypal.com/sdk/js?client-id=AR-QXmPS8cQH39UcJhoQlcC4q_R1yS75dA6_CYfjGXjNLOdtaon12aRbqqcv3YBM_Brh7vK0KtP_Rxvg&vault=true" data-sdk-integration-source="button-factory"></script>
<script>
  paypal.Buttons({
      style: {
          shape: 'rect',
          color: 'blue',
          layout: 'vertical',
          label: 'subscribe'
      },
      createSubscription: function(data, actions) {
        return actions.subscription.create({
          'plan_id': 'P-1LB35144FS508802VL5U2NII'
        });
      },
      onApprove: function(data, actions) {
        alert(data.subscriptionID);
      }
  }).render('#paypal-button-container');
</script>