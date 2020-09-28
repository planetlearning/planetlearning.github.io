<div id="paypal-button-container"></div>
<script src="https://www.paypal.com/sdk/js?client-id=AR-QXmPS8cQH39UcJhoQlcC4q_R1yS75dA6_CYfjGXjNLOdtaon12aRbqqcv3YBM_Brh7vK0KtP_Rxvg&vault=true" data-sdk-integration-source="button-factory"></script>
<script>
  $(document).ready(function() {
  paypal.Buttons({
      style: {
          shape: 'rect',
          color: 'blue',
          layout: 'vertical',
          label: 'paypal'
      },
      createSubscription: function(data, actions) {
        return actions.subscription.create({
          'plan_id': 'P-9XN71522E8186850BL5ZAF4A'
        });
      },
      onApprove: function(data, actions) {
        alert(data.subscriptionID);
      }
  }).render('#paypal-button-container');
  });
</script>