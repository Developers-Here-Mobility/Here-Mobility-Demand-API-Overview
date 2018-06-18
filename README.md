<!DOCTYPE html>

<html>
  <head>
    <title>Protocol Documentation</title>
    <meta charset="UTF-8">
    <link rel="stylesheet" type="text/css" href="http://fonts.googleapis.com/css?family=Ubuntu:400,700,400italic"/>
    <style>
      body {
        width: 60em;
        margin: 1em auto;
        color: #222;
        font-family: "Ubuntu", sans-serif;
        padding-bottom: 4em;
      }

      h1 {
        font-weight: normal;
        border-bottom: 1px solid #aaa;
        padding-bottom: 0.5ex;
      }

      h2 {
        border-bottom: 1px solid #aaa;
        padding-bottom: 0.5ex;
        margin: 1.5em 0;
      }

      h3 {
        font-weight: normal;
        border-bottom: 1px solid #aaa;
        padding-bottom: 0.5ex;
      }

      a {
        text-decoration: none;
        color: #567e25;
      }

      table {
        width: 100%;
        font-size: 80%;
        border-collapse: collapse;
      }

      thead {
        font-weight: 700;
        background-color: #dcdcdc;
      }

      tbody tr:nth-child(even) {
        background-color: #fbfbfb;
      }

      td {
        border: 1px solid #ccc;
        padding: 0.5ex 2ex;
      }

      td p {
        text-indent: 1em;
        margin: 0;
      }

      td p:nth-child(1) {
        text-indent: 0;  
      }

       
      .field-table td:nth-child(1) {  
        width: 10em;
      }
      .field-table td:nth-child(2) {  
        width: 10em;
      }
      .field-table td:nth-child(3) {  
        width: 6em;
      }
      .field-table td:nth-child(4) {  
        width: auto;
      }

       
      .extension-table td:nth-child(1) {  
        width: 10em;
      }
      .extension-table td:nth-child(2) {  
        width: 10em;
      }
      .extension-table td:nth-child(3) {  
        width: 10em;
      }
      .extension-table td:nth-child(4) {  
        width: 5em;
      }
      .extension-table td:nth-child(5) {  
        width: auto;
      }

       
      .enum-table td:nth-child(1) {  
        width: 10em;
      }
      .enum-table td:nth-child(2) {  
        width: 10em;
      }
      .enum-table td:nth-child(3) {  
        width: auto;
      }

       
      .scalar-value-types-table tr {
        height: 3em;
      }

       
      #toc-container ul {
        list-style-type: none;
        padding-left: 1em;
        line-height: 180%;
        margin: 0;
      }
      #toc > li > a {
        font-weight: bold;
      }

       
      .file-heading {
        width: 100%;
        display: table;
        border-bottom: 1px solid #aaa;
        margin: 4em 0 1.5em 0;
      }
      .file-heading h2 {
        border: none;
        display: table-cell;
      }
      .file-heading a {
        text-align: right;
        display: table-cell;
      }

       
      .badge {
        width: 1.6em;
        height: 1.6em;
        display: inline-block;

        line-height: 1.6em;
        text-align: center;
        font-weight: bold;
        font-size: 60%;

        color: #89ba48;
        background-color: #dff0c8;

        margin: 0.5ex 1em 0.5ex -1em;
        border: 1px solid #fbfbfb;
        border-radius: 1ex;
      }
    </style>

    
    <link rel="stylesheet" type="text/css" href="stylesheet.css"/>
  </head>

  <body>

    <h1 id="title">Protocol Documentation</h1>

    <h2>Table of Contents</h2>

    <div id="toc-container">
      <ul id="toc">
        
          
          <li>
            <a href="#marketplace%2fpublic%2fgrpc%2fdemand_handler%2fv2%2fgen-doc%2fdemand_c2s_messages.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_c2s_messages.proto</a>
            <ul>
              
                <li>
                  <a href="#demand.v2.c2s.CancelRideRequest"><span class="badge">M</span>CancelRideRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.c2s.CreatePublicTransportRideRequest"><span class="badge">M</span>CreatePublicTransportRideRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.c2s.CreateRideRequest"><span class="badge">M</span>CreateRideRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.c2s.GetRideListRequest"><span class="badge">M</span>GetRideListRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.c2s.GetRideLocationRequest"><span class="badge">M</span>GetRideLocationRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.c2s.GetRideRequest"><span class="badge">M</span>GetRideRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.c2s.RideOffersRequest"><span class="badge">M</span>RideOffersRequest</a>
                </li>
              
              
              
              
            </ul>
          </li>
        
          
          <li>
            <a href="#marketplace%2fpublic%2fgrpc%2fdemand_handler%2fv2%2fgen-doc%2fdemand_c2s_service.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_c2s_service.proto</a>
            <ul>
              
              
              
              
                <li>
                  <a href="#demand.v2.c2s.C2SDemandApi"><span class="badge">S</span>C2SDemandApi</a>
                </li>
              
            </ul>
          </li>
        
          
          <li>
            <a href="#marketplace%2fpublic%2fgrpc%2fdemand_handler%2fv2%2fgen-doc%2fdemand_common_entities.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_common_entities.proto</a>
            <ul>
              
                <li>
                  <a href="#demand.v2.common.BookingConstraints"><span class="badge">M</span>BookingConstraints</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.CancellationInfo"><span class="badge">M</span>CancellationInfo</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.DriverDetails"><span class="badge">M</span>DriverDetails</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.PassengerDetails"><span class="badge">M</span>PassengerDetails</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.PublicTransportRouteLeg"><span class="badge">M</span>PublicTransportRouteLeg</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.Ride"><span class="badge">M</span>Ride</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideLocation"><span class="badge">M</span>RideLocation</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideOffer"><span class="badge">M</span>RideOffer</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideOffersResponse"><span class="badge">M</span>RideOffersResponse</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideQuery"><span class="badge">M</span>RideQuery</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideQueryResponse"><span class="badge">M</span>RideQueryResponse</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideStatusLog"><span class="badge">M</span>RideStatusLog</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideStatusUpdate"><span class="badge">M</span>RideStatusUpdate</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.Route"><span class="badge">M</span>Route</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.Supplier"><span class="badge">M</span>Supplier</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.TransitOptions"><span class="badge">M</span>TransitOptions</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.Vehicle"><span class="badge">M</span>Vehicle</a>
                </li>
              
              
                <li>
                  <a href="#demand.v2.common.CancellationInfo.Party"><span class="badge">E</span>CancellationInfo.Party</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.CancellationInfo.Status"><span class="badge">E</span>CancellationInfo.Status</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.PublicTransportRouteLeg.PublicTransportMode"><span class="badge">E</span>PublicTransportRouteLeg.PublicTransportMode</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideOffer.CancellationPolicy"><span class="badge">E</span>RideOffer.CancellationPolicy</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideOffer.SortType"><span class="badge">E</span>RideOffer.SortType</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideOffer.TransitType"><span class="badge">E</span>RideOffer.TransitType</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideQuery.RideStatusFilter"><span class="badge">E</span>RideQuery.RideStatusFilter</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideQuery.SortType"><span class="badge">E</span>RideQuery.SortType</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.RideStatusUpdate.Status"><span class="badge">E</span>RideStatusUpdate.Status</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.Vehicle.VehicleType"><span class="badge">E</span>Vehicle.VehicleType</a>
                </li>
              
              
              
            </ul>
          </li>
        
          
          <li>
            <a href="#marketplace%2fpublic%2fgrpc%2fdemand_handler%2fv2%2fgen-doc%2fdemand_common_types.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_common_types.proto</a>
            <ul>
              
                <li>
                  <a href="#demand.v2.common.Address"><span class="badge">M</span>Address</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.Empty"><span class="badge">M</span>Empty</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.Location"><span class="badge">M</span>Location</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.Point"><span class="badge">M</span>Point</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.Price"><span class="badge">M</span>Price</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.PriceEstimate"><span class="badge">M</span>PriceEstimate</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.PriceRange"><span class="badge">M</span>PriceRange</a>
                </li>
              
                <li>
                  <a href="#demand.v2.common.TimeRange"><span class="badge">M</span>TimeRange</a>
                </li>
              
              
              
              
            </ul>
          </li>
        
          
          <li>
            <a href="#marketplace%2fpublic%2fgrpc%2fdemand_handler%2fv2%2fgen-doc%2fdemand_s2s_messages.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_s2s_messages.proto</a>
            <ul>
              
                <li>
                  <a href="#demand.v2.s2s.CancelRideRequest"><span class="badge">M</span>CancelRideRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.s2s.CreatePublicTransportRideRequest"><span class="badge">M</span>CreatePublicTransportRideRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.s2s.CreateRideRequest"><span class="badge">M</span>CreateRideRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.s2s.GetRecentRidesRequest"><span class="badge">M</span>GetRecentRidesRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.s2s.GetRideListByUserRequest"><span class="badge">M</span>GetRideListByUserRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.s2s.GetRideListRequest"><span class="badge">M</span>GetRideListRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.s2s.GetRideLocationRequest"><span class="badge">M</span>GetRideLocationRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.s2s.GetRideRequest"><span class="badge">M</span>GetRideRequest</a>
                </li>
              
                <li>
                  <a href="#demand.v2.s2s.RideOffersRequest"><span class="badge">M</span>RideOffersRequest</a>
                </li>
              
              
              
              
            </ul>
          </li>
        
          
          <li>
            <a href="#marketplace%2fpublic%2fgrpc%2fdemand_handler%2fv2%2fgen-doc%2fdemand_s2s_service.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_s2s_service.proto</a>
            <ul>
              
              
              
              
                <li>
                  <a href="#demand.v2.s2s.S2SDemandApi"><span class="badge">S</span>S2SDemandApi</a>
                </li>
              
            </ul>
          </li>
        
        <li><a href="#scalar-value-types">Scalar Value Types</a></li>
      </ul>
    </div>

    
      
      <div class="file-heading">
        <h2 id="marketplace/public/grpc/demand_handler/v2/gen-doc/demand_c2s_messages.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_c2s_messages.proto</h2><a href="#title">Top</a>
      </div>
      <p></p>

      
        <h3 id="demand.v2.c2s.CancelRideRequest">CancelRideRequest</h3>
        <p>A request to cancel a ride</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>ride_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. The unique ride ID </p></td>
                </tr>
              
                <tr>
                  <td>cancel_reason</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Optional. Free text. The reason for the cancellation. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.c2s.CreatePublicTransportRideRequest">CreatePublicTransportRideRequest</h3>
        <p></p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>offer</td>
                  <td><a href="#demand.v2.common.RideOffer">demand.v2.common.RideOffer</a></td>
                  <td></td>
                  <td><p>Mandatory. The chosen public transportation offer. </p></td>
                </tr>
              
                <tr>
                  <td>passenger</td>
                  <td><a href="#demand.v2.common.PassengerDetails">demand.v2.common.PassengerDetails</a></td>
                  <td></td>
                  <td><p>Mandatory. The passenger details at the time of booking </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.c2s.CreateRideRequest">CreateRideRequest</h3>
        <p>A request to create a new ride by offer ID</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>offer_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. An offer ID that was returned by GetRideOffers() </p></td>
                </tr>
              
                <tr>
                  <td>passenger</td>
                  <td><a href="#demand.v2.common.PassengerDetails">demand.v2.common.PassengerDetails</a></td>
                  <td></td>
                  <td><p>Mandatory. The passenger details at the time of booking </p></td>
                </tr>
              
                <tr>
                  <td>subscribe_to_messages</td>
                  <td><a href="#google.protobuf.BoolValue">google.protobuf.BoolValue</a></td>
                  <td></td>
                  <td><p>Optional. Specifies if messages about the ride will be sent to the passenger. Default is true. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.c2s.GetRideListRequest">GetRideListRequest</h3>
        <p>A request to get a ride list according to query parameters.</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>query</td>
                  <td><a href="#demand.v2.common.RideQuery">demand.v2.common.RideQuery</a></td>
                  <td></td>
                  <td><p>Optional. The query parameters with which to filter the rides returned.
If no query parameters are supplied, the query uses the default values for RideQuery fields (see the RideQuery message documentation). </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.c2s.GetRideLocationRequest">GetRideLocationRequest</h3>
        <p></p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>ride_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. The ride’s unique ID </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.c2s.GetRideRequest">GetRideRequest</h3>
        <p>A request to get a ride</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>ride_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. The ride’s unique ID </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.c2s.RideOffersRequest">RideOffersRequest</h3>
        <p>A request to get ride offers for a given route. If a prebook_pickup_time value is provided, this is a request for a future pickup.</p><p>Otherwise, this is a request for an immediate pickup (within 30 minutes).</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>route</td>
                  <td><a href="#demand.v2.common.Route">demand.v2.common.Route</a></td>
                  <td></td>
                  <td><p>Mandatory. The requested route of the ride. </p></td>
                </tr>
              
                <tr>
                  <td>constraints</td>
                  <td><a href="#demand.v2.common.BookingConstraints">demand.v2.common.BookingConstraints</a></td>
                  <td></td>
                  <td><p>Optional. Ride constraints such as passenger count, child seats, number of suitcases, etc. </p></td>
                </tr>
              
                <tr>
                  <td>prebook_pickup_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Optional. An optional future pickup time, which is at least 30 minutes after the request time.
An empty value indicates a request for an immediate ride. </p></td>
                </tr>
              
                <tr>
                  <td>price_range</td>
                  <td><a href="#demand.v2.common.PriceRange">demand.v2.common.PriceRange</a></td>
                  <td></td>
                  <td><p>Optional, unsupported. An optional requested price range. If this value is set, only offers
whose price is within the range are returned. Otherwise, any price is assumed to be acceptable. </p></td>
                </tr>
              
                <tr>
                  <td>sort_type</td>
                  <td><a href="#demand.v2.common.RideOffer.SortType">demand.v2.common.RideOffer.SortType</a></td>
                  <td></td>
                  <td><p>FUTURE FEATURE, CURRENTLY UNSUPPORTED: Optional. How to sort the RideOffers, by price or by ETA.
(The Marketplace default sort order is by best price, and then minimal ETA.) </p></td>
                </tr>
              
                <tr>
                  <td>passenger_note</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Optional. A free text note from the passenger. </p></td>
                </tr>
              
                <tr>
                  <td>instance_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Optional. The ID of the instance. </p></td>
                </tr>
              
                <tr>
                  <td>transit_options</td>
                  <td><a href="#demand.v2.common.TransitOptions">demand.v2.common.TransitOptions</a></td>
                  <td></td>
                  <td><p>Optional. Parameters for transit offers. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      

      

      

      
    
      
      <div class="file-heading">
        <h2 id="marketplace/public/grpc/demand_handler/v2/gen-doc/demand_c2s_service.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_c2s_service.proto</h2><a href="#title">Top</a>
      </div>
      <p>The client 2 service api</p>

      

      

      

      
        <h3 id="demand.v2.c2s.C2SDemandApi">C2SDemandApi</h3>
        <p>A service-to-service API for creating and tracking rides.</p><p>All ride-related entities are created for the current user. The user (or session) is included in the header of all requests.</p><p>=== Normal flow before the ride is created ===</p><p>The client calls GetRideOffers() according to the time, route, price and other constraints that the user specifies.</p><p>The user chooses one ride offer, and the client calls Book().</p><p>The client calls GetRide() repeatedly until the ride status is ACCEPTED.</p><p>=== Normal flow during the ride ===</p><p>The client calls GetRide() repeatedly to get ride status updates.</p><p>The client calls GetRideLocation() repeatedly to get ride location and ETA updates. These calls should be made more frequently, as the location changes continuously.</p><p>=== Flow for getting updates on multiple rides ===</p><p>The client makes an initial call to GetRides() to receive recently updated rides.</p><p>The client repeatedly calls GetRides() to get new updates. Starting from the second call to GetRides(), send the 'to_update_time' from the previous response as the requested minimal update time.</p><p>==== Errors ===</p><p>- NOT_FOUND code – may be returned when an entity doesn’t exist, is expired (such as an offer) or belongs to a different user.</p><p>=== Future Enhancments ===</p><p>Optimization of polling (using ETAG)</p><p>History of rides</p>
        <table class="enum-table">
          <thead>
            <tr><td>Method Name</td><td>Request Type</td><td>Response Type</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>GetRideOffers</td>
                <td><a href="#demand.v2.c2s.RideOffersRequest">RideOffersRequest</a></td>
                <td><a href="#demand.v2.common.RideOffersResponse">.demand.v2.common.RideOffersResponse</a></td>
                <td><p>Get ride offers based on a ride request. May take a few seconds. When no offers are available, returns an empty response.
Errors:
INVALID_ARGUMENT: Invalid field value. For example: prebook_pickup_time is in the past, route.pickup.lat is not a valid latitude, etc.</p></td>
              </tr>
            
              <tr>
                <td>CreateRide</td>
                <td><a href="#demand.v2.c2s.CreateRideRequest">CreateRideRequest</a></td>
                <td><a href="#demand.v2.common.Ride">.demand.v2.common.Ride</a></td>
                <td><p>Create a new ride based on an offer ID. If the offer is valid, a ride is returned immediately with the status PROCESSING.

Errors:
NOT_FOUND: The offer ID is expired or does not exist
ALREADY_EXISTS: A booking already exists for this offer ID (call GetRideOffers to receive new offer IDs).</p></td>
              </tr>
            
              <tr>
                <td>GetRide</td>
                <td><a href="#demand.v2.c2s.GetRideRequest">GetRideRequest</a></td>
                <td><a href="#demand.v2.common.Ride">.demand.v2.common.Ride</a></td>
                <td><p>Get a ride by ID. Use this call to poll for the ride status (every 10 seconds).
NOTE: The status of closed rides (COMPLETED, CANCELLED, REJECTED) never changes.
Errors: 
NOT_FOUND: Ride does not exist</p></td>
              </tr>
            
              <tr>
                <td>GetRides</td>
                <td><a href="#demand.v2.c2s.GetRideListRequest">GetRideListRequest</a></td>
                <td><a href="#demand.v2.common.RideQueryResponse">.demand.v2.common.RideQueryResponse</a></td>
                <td><p>Get rides for the current user.
Returns rides that were updated recently (in the last 3 hours, or after the given from_update_time).</p></td>
              </tr>
            
              <tr>
                <td>CancelRide</td>
                <td><a href="#demand.v2.c2s.CancelRideRequest">CancelRideRequest</a></td>
                <td><a href="#demand.v2.common.Empty">.demand.v2.common.Empty</a></td>
                <td><p>Cancel a ride. Returns immediately without waiting for a response from the supplier.
Errors:
NOT_FOUND: Ride does not exist
FAILED_PRECONDITION: Cancel is not allowed by policy, or because the status is REJECTED, COMPLETED, or CANCELLED.</p></td>
              </tr>
            
              <tr>
                <td>GetRideLocationAndEta</td>
                <td><a href="#demand.v2.c2s.GetRideLocationRequest">GetRideLocationRequest</a></td>
                <td><a href="#demand.v2.common.RideLocation">.demand.v2.common.RideLocation</a></td>
                <td><p>Returns the geo-location of the ride. Use this call to poll for the ride location (every 10 seconds)
NOTES:
Test the flag Ride.status_log.is_ride_location_available, to learn whether ride locations are supported.
Rides which are closed (COMPLETED, CANCELLED, REJECTED) never change their location.
Errors:
NOT_FOUND: Ride does not exist</p></td>
              </tr>
            
              <tr>
                <td>CreatePublicTransportRide</td>
                <td><a href="#demand.v2.c2s.CreatePublicTransportRideRequest">CreatePublicTransportRideRequest</a></td>
                <td><a href="#demand.v2.common.Empty">.demand.v2.common.Empty</a></td>
                <td><p>Notify the marketplace that a public transportation offer was chosen</p></td>
              </tr>
            
          </tbody>
        </table>
      
    
      
      <div class="file-heading">
        <h2 id="marketplace/public/grpc/demand_handler/v2/gen-doc/demand_common_entities.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_common_entities.proto</h2><a href="#title">Top</a>
      </div>
      <p>Common entities, such as Route, Ride and RideOffer</p>

      
        <h3 id="demand.v2.common.BookingConstraints">BookingConstraints</h3>
        <p>A structure for defining the number of passengers and special requirements for the ride.</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>passengers_no</td>
                  <td><a href="#uint32">uint32</a></td>
                  <td></td>
                  <td><p>The number of passengers (1 or more) </p></td>
                </tr>
              
                <tr>
                  <td>suitcases_no</td>
                  <td><a href="#uint32">uint32</a></td>
                  <td></td>
                  <td><p>The number of suitcases (0 or more) </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.CancellationInfo">CancellationInfo</h3>
        <p>Information about a ride cancellation</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>cancelling_party</td>
                  <td><a href="#demand.v2.common.CancellationInfo.Party">CancellationInfo.Party</a></td>
                  <td></td>
                  <td><p>Which party canceled the ride </p></td>
                </tr>
              
                <tr>
                  <td>cancel_reason</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The reason the ride was canceled (a free-text string) </p></td>
                </tr>
              
                <tr>
                  <td>request_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>The time the cancellation was requested </p></td>
                </tr>
              
                <tr>
                  <td>status</td>
                  <td><a href="#demand.v2.common.CancellationInfo.Status">CancellationInfo.Status</a></td>
                  <td></td>
                  <td><p>The status of the cancellation request </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.DriverDetails">DriverDetails</h3>
        <p>Driver information</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>name</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The driver’s first and last name </p></td>
                </tr>
              
                <tr>
                  <td>phone_number</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The driver’s telephone number </p></td>
                </tr>
              
                <tr>
                  <td>photo_url</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>A URL pointing to the driver’s photo. This is mandatory in some countries. </p></td>
                </tr>
              
                <tr>
                  <td>driving_license_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The driver’s driving license ID. This is mandatory in some countries. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.PassengerDetails">PassengerDetails</h3>
        <p>Passenger information</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>name</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. The passenger’s first and last name </p></td>
                </tr>
              
                <tr>
                  <td>phone_number</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The passenger’s telephone number </p></td>
                </tr>
              
                <tr>
                  <td>photo_url</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Optional. A URL pointing to the passenger’s photo. </p></td>
                </tr>
              
                <tr>
                  <td>email</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Optional. An email address to contact the passenger. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.PublicTransportRouteLeg">PublicTransportRouteLeg</h3>
        <p></p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>mode</td>
                  <td><a href="#demand.v2.common.PublicTransportRouteLeg.PublicTransportMode">PublicTransportRouteLeg.PublicTransportMode</a></td>
                  <td></td>
                  <td><p>Type of transportation for the leg </p></td>
                </tr>
              
                <tr>
                  <td>duration_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Duration of the leg in milliseconds </p></td>
                </tr>
              
                <tr>
                  <td>distance_meters</td>
                  <td><a href="#uint32">uint32</a></td>
                  <td></td>
                  <td><p>Distance of the leg in meters </p></td>
                </tr>
              
                <tr>
                  <td>line</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Name of the line of this public transportation, if the leg is a public transportation leg </p></td>
                </tr>
              
                <tr>
                  <td>origin</td>
                  <td><a href="#demand.v2.common.Location">Location</a></td>
                  <td></td>
                  <td><p>Origin location of the leg </p></td>
                </tr>
              
                <tr>
                  <td>departure_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Time of departure from the start of the leg in milliseconds </p></td>
                </tr>
              
                <tr>
                  <td>destination</td>
                  <td><a href="#demand.v2.common.Location">Location</a></td>
                  <td></td>
                  <td><p>Destination location of the leg </p></td>
                </tr>
              
                <tr>
                  <td>arrival_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Time of arrival from the start of the leg in milliseconds </p></td>
                </tr>
              
                <tr>
                  <td>operator</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Name of the public transportion operator for this leg </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.Ride">Ride</h3>
        <p>A ride with a specific supplier. This entity contains relatively static info: driver, vehicle, passengers etc.</p><p>The more dynamic info of the ride, including its progress along the route, is in the entity Ride.</p><p>Below is the lifecycle of the ride:</p><p>PROCESSING [initial status of the ride after CreateRide(). 0-15 sec]</p><p>PROCESSING --> ACCEPTED [For a pre-booked ride, this status will be active until 30min before the ride]</p><p>PROCESSING --> REJECTED [The ride has been rejected. Terminal state]</p><p>ACCEPTED --> PROCESSING [This state occurs if the supplier cancels a pre-booked ride, and the Marketplace tries to book a new ride.]</p><p>ACCEPTED --> ((NORMAL FLOW)) --> COMPLETE [The ride has been completed. Terminal state.]</p><p>The typical flow is: DRIVER_ASSIGNED --> DRIVER_EN_ROUTE --> AT_PICKUP --> PASSENGER_ON_BOARD --> AT_DROPOFF</p><p>CANCELLED [Terminal state. Can be reached from any other state, if a demander or supplier cancels the ride.]</p><p>NOTE: Once a ride reaches a terminal state, it cannot transition to any other state.</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>user_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The ID of the user who created this ride </p></td>
                </tr>
              
                <tr>
                  <td>ride_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>A unique ride id </p></td>
                </tr>
              
                <tr>
                  <td>route</td>
                  <td><a href="#demand.v2.common.Route">Route</a></td>
                  <td></td>
                  <td><p>The ride route </p></td>
                </tr>
              
                <tr>
                  <td>prebook_pickup_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Optional. For a pre-booked ride, contains the requested pickup time. </p></td>
                </tr>
              
                <tr>
                  <td>booking_estimated_price</td>
                  <td><a href="#demand.v2.common.PriceEstimate">PriceEstimate</a></td>
                  <td></td>
                  <td><p>The estimated price at the time of booking. </p></td>
                </tr>
              
                <tr>
                  <td>constraints</td>
                  <td><a href="#demand.v2.common.BookingConstraints">BookingConstraints</a></td>
                  <td></td>
                  <td><p>Constraints defined at the time of booking, such as number of passengers and suitcases. </p></td>
                </tr>
              
                <tr>
                  <td>status_log</td>
                  <td><a href="#demand.v2.common.RideStatusLog">RideStatusLog</a></td>
                  <td></td>
                  <td><p>The ride’s current status, and status history. </p></td>
                </tr>
              
                <tr>
                  <td>supplier</td>
                  <td><a href="#demand.v2.common.Supplier">Supplier</a></td>
                  <td></td>
                  <td><p>Supplier details </p></td>
                </tr>
              
                <tr>
                  <td>passenger</td>
                  <td><a href="#demand.v2.common.PassengerDetails">PassengerDetails</a></td>
                  <td></td>
                  <td><p>The passenger details at the time of ride creation </p></td>
                </tr>
              
                <tr>
                  <td>passenger_note</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Optional. A note added by the passenger at the time of ride creation. Can include additional information about the pickup or other special requests. </p></td>
                </tr>
              
                <tr>
                  <td>driver</td>
                  <td><a href="#demand.v2.common.DriverDetails">DriverDetails</a></td>
                  <td></td>
                  <td><p>Optional. This field is only filled when the ride status changes to DRIVER_ASSIGNED and after. </p></td>
                </tr>
              
                <tr>
                  <td>vehicle</td>
                  <td><a href="#demand.v2.common.Vehicle">Vehicle</a></td>
                  <td></td>
                  <td><p>Optional. This field is only filled when the ride status changes to DRIVER_ASSIGNED and after. </p></td>
                </tr>
              
                <tr>
                  <td>cancellation_policy</td>
                  <td><a href="#demand.v2.common.RideOffer.CancellationPolicy">RideOffer.CancellationPolicy</a></td>
                  <td></td>
                  <td><p>The cancellation policy for the ride </p></td>
                </tr>
              
                <tr>
                  <td>cancellation_info</td>
                  <td><a href="#demand.v2.common.CancellationInfo">CancellationInfo</a></td>
                  <td></td>
                  <td><p>Optional. When a cancellation occurs, this field contains information about the cancellation. </p></td>
                </tr>
              
                <tr>
                  <td>cancellation_request_received_but_not_allowed</td>
                  <td><a href="#bool">bool</a></td>
                  <td></td>
                  <td><p>When a cancellation occurs, this field value is TRUE if cancellation isn&#39;t allowed </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.RideLocation">RideLocation</h3>
        <p>Provides the real-time location and progress of the vehicle. Updated every ~10 seconds.</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>ride_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The ID of the ride. </p></td>
                </tr>
              
                <tr>
                  <td>vehicle_location</td>
                  <td><a href="#demand.v2.common.Point">Point</a></td>
                  <td></td>
                  <td><p>Optional. The current location of the vehicle. </p></td>
                </tr>
              
                <tr>
                  <td>estimated_pickup_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Optional. The estimated time of pickup, constantly updated until the vehicle is at the pickup location. </p></td>
                </tr>
              
                <tr>
                  <td>estimated_dropoff_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Optional. The estimated time of drop-off, constantly updated until the vehicle is at the drop-off location. </p></td>
                </tr>
              
                <tr>
                  <td>last_update_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>The last time this entity is updated. Used for tracking updates. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.RideOffer">RideOffer</h3>
        <p>An offer for a ride on the given route.</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>offer_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>A unique offer ID. If this offer is chosen, the client sends this ID when calling CreateRide. </p></td>
                </tr>
              
                <tr>
                  <td>supplier</td>
                  <td><a href="#demand.v2.common.Supplier">Supplier</a></td>
                  <td></td>
                  <td><p>The supplier details </p></td>
                </tr>
              
                <tr>
                  <td>route</td>
                  <td><a href="#demand.v2.common.Route">Route</a></td>
                  <td></td>
                  <td><p>The ride route that the supplier suggests. </p></td>
                </tr>
              
                <tr>
                  <td>estimated_pickup_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Optional. Pickup time estimate sent by the supplier. </p></td>
                </tr>
              
                <tr>
                  <td>estimated_dropoff_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Optional. Drop-off time estimate sent by the supplier. </p></td>
                </tr>
              
                <tr>
                  <td>price_estimation</td>
                  <td><a href="#demand.v2.common.PriceEstimate">PriceEstimate</a></td>
                  <td></td>
                  <td><p>Optional. A price estimate for the ride </p></td>
                </tr>
              
                <tr>
                  <td>offer_expiration_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>The offer expiration time in milliseconds </p></td>
                </tr>
              
                <tr>
                  <td>cancellation_policy</td>
                  <td><a href="#demand.v2.common.RideOffer.CancellationPolicy">RideOffer.CancellationPolicy</a></td>
                  <td></td>
                  <td><p>The cancellation policy of the supplier (cancellation allowed or not allowed) </p></td>
                </tr>
              
                <tr>
                  <td>duration_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Duration of the route in milliseconds </p></td>
                </tr>
              
                <tr>
                  <td>transfers</td>
                  <td><a href="#uint32">uint32</a></td>
                  <td></td>
                  <td><p>Number of transport changes to reach the destination </p></td>
                </tr>
              
                <tr>
                  <td>legs</td>
                  <td><a href="#demand.v2.common.PublicTransportRouteLeg">PublicTransportRouteLeg</a></td>
                  <td>repeated</td>
                  <td><p>A list of transportation legs for the route, if this offer is a public transportation offer </p></td>
                </tr>
              
                <tr>
                  <td>transit_type</td>
                  <td><a href="#demand.v2.common.RideOffer.TransitType">RideOffer.TransitType</a></td>
                  <td></td>
                  <td><p>Specifies the transit type of this offer </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.RideOffersResponse">RideOffersResponse</h3>
        <p>A list of available ride offers</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>offers</td>
                  <td><a href="#demand.v2.common.RideOffer">RideOffer</a></td>
                  <td>repeated</td>
                  <td><p>A list of ride offers </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.RideQuery">RideQuery</h3>
        <p>A query for range of rides. Used as request for GetRides() and supports pagination, sorting and filtering.</p><p>To fetch a next page, simply copy the pagination field from the response to the next GetRides() request:</p><p>next_request.from_time_ms = response.to_time_ms</p><p>Paging can be used in 2 ways: ENDLESS PAGING and SINGLE SNAPSHOT (more below).</p><p>Also note that when the sort is by CREATE_TIME (asc or desc), rides never repeat between pages.</p><p>when the sort is UPDATE_TIME (asc or desc), rides in previous pages can appear again (because of updates).</p><p>when the sort is PICKUP_TIME (asc or desc), rides in previous pages can appear again, but rarely.</p><p>ENDLESS PAGING - relevant for ascending sorts.</p><p>In this mode, the client should call GetRides() in regular intervals to recieve new or updated records.</p><p>The sort UPDATE_TIME_ASC, can be used to recieve all changes on rides</p><p>The sort CREATE_TIME_ASC can be used to recieve each ride exactly once (without updates).</p><p>The sort PICKUP_TIME_ASC is similar to CREATE_TIME_ASC and is useful to page future rides.</p><p>SINGLE SNAPSHOT - in this mode, the client wants to fetch all the rides, and needs to know what is the last page.</p><p>To identify the last page, set the 'limit' field in the RideQuery, and check if the amount of rides in the result</p><p>is lower than the limit. By default any result with less than 200 rides is the last page.</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>from_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Optional. Return rides equal or greater than this value according to sort type.
when the sort is UPDATE_TIME_ASC, returns rides UPDATED AFTER this time.
when the sort is CREATE_TIME_DESC, return rides CREATED BEFORE this time.
etc.
Default value for ASC sorts is NOW-3hours.
Default value for DESC sorts is NOW.
This value is in utc (milliseconds since epoch time) </p></td>
                </tr>
              
                <tr>
                  <td>limit</td>
                  <td><a href="#uint32">uint32</a></td>
                  <td></td>
                  <td><p>Optional. The maximal number of rides to return. When not set, the default is 200. </p></td>
                </tr>
              
                <tr>
                  <td>status_filter</td>
                  <td><a href="#demand.v2.common.RideQuery.RideStatusFilter">RideQuery.RideStatusFilter</a></td>
                  <td></td>
                  <td><p>Optional. Return only rides with the given status. When not set, rides with all statuses are returned. </p></td>
                </tr>
              
                <tr>
                  <td>sort_by</td>
                  <td><a href="#demand.v2.common.RideQuery.SortType">RideQuery.SortType</a></td>
                  <td></td>
                  <td><p>Optional. Default is UPDATE_TIME_ASC. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.RideQueryResponse">RideQueryResponse</h3>
        <p>A list of rides that matches a ride query</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>rides</td>
                  <td><a href="#demand.v2.common.Ride">Ride</a></td>
                  <td>repeated</td>
                  <td><p>The list of rides that matched the query </p></td>
                </tr>
              
                <tr>
                  <td>from_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>The earliest update time in this result set. The lowest possible value is current time minus 3 hours.
This value is in UTC, in milliseconds since Epoch time. </p></td>
                </tr>
              
                <tr>
                  <td>to_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>A cursor for pagination. Contains the last time in the result set, ordered by the sort type.
To get the next page, pass this value to the next call for GetRides() to field RideQuery.from_time_ms
This value is in UTC, in milliseconds since Epoch time. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.RideStatusLog">RideStatusLog</h3>
        <p>The current status of the ride, including some audit info, and a history of previous statuses</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>last_update_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>The last time this entity was updated. Used for tracking updates. </p></td>
                </tr>
              
                <tr>
                  <td>create_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>The time the booking was created </p></td>
                </tr>
              
                <tr>
                  <td>closed_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Optional. If relevant, the time the ride was closed. </p></td>
                </tr>
              
                <tr>
                  <td>is_ride_location_available</td>
                  <td><a href="#bool">bool</a></td>
                  <td></td>
                  <td><p>If this value is TRUE, you can retrieve live updates on the ride’s location by calling GetRideLocation (during statuses DRIVER_ASSIGNED to COMPLETED) </p></td>
                </tr>
              
                <tr>
                  <td>current_status</td>
                  <td><a href="#demand.v2.common.RideStatusUpdate.Status">RideStatusUpdate.Status</a></td>
                  <td></td>
                  <td><p>The ride’s current status </p></td>
                </tr>
              
                <tr>
                  <td>prev_statuses</td>
                  <td><a href="#demand.v2.common.RideStatusUpdate">RideStatusUpdate</a></td>
                  <td>repeated</td>
                  <td><p>A list of previous ride statuses, ordered by their timestamp values. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.RideStatusUpdate">RideStatusUpdate</h3>
        <p>A ride status update, and the time it occurred. Used in the status log.</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>status</td>
                  <td><a href="#demand.v2.common.RideStatusUpdate.Status">RideStatusUpdate.Status</a></td>
                  <td></td>
                  <td><p>The new ride status </p></td>
                </tr>
              
                <tr>
                  <td>timestamp_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>The time the ride status changed (UNIX Epoch time in milliseconds). </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.Route">Route</h3>
        <p>A route between a start point and an end point</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>pickup</td>
                  <td><a href="#demand.v2.common.Location">Location</a></td>
                  <td></td>
                  <td><p>Mandatory. The route’s pickup location. </p></td>
                </tr>
              
                <tr>
                  <td>destination</td>
                  <td><a href="#demand.v2.common.Location">Location</a></td>
                  <td></td>
                  <td><p>Mandatory. The route’s destination location. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.Supplier">Supplier</h3>
        <p>Ride supplier details</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>supplier_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>A unique supplier ID </p></td>
                </tr>
              
                <tr>
                  <td>english_name</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The name of the supplier, in English </p></td>
                </tr>
              
                <tr>
                  <td>local_name</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Optional. The name of the supplier in the local language </p></td>
                </tr>
              
                <tr>
                  <td>logo_url</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Optional. A URL pointing to a logo image for the supplier </p></td>
                </tr>
              
                <tr>
                  <td>phone_number</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The supplier’s telephone number </p></td>
                </tr>
              
                <tr>
                  <td>address</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The supplier’s address </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.TransitOptions">TransitOptions</h3>
        <p></p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>max_transfers</td>
                  <td><a href="#google.protobuf.Int32Value">google.protobuf.Int32Value</a></td>
                  <td></td>
                  <td><p>Optional. Maximum number of changes or transfers allowed in a route. Default is unlimited. Range is 0-6. </p></td>
                </tr>
              
                <tr>
                  <td>max_walking_distance_meters</td>
                  <td><a href="#google.protobuf.Int32Value">google.protobuf.Int32Value</a></td>
                  <td></td>
                  <td><p>Optional. Specifies a maximum walking distance in meters. Default is 2000. Range is 0-6000. </p></td>
                </tr>
              
                <tr>
                  <td>locale</td>
                  <td><a href="#google.protobuf.StringValue">google.protobuf.StringValue</a></td>
                  <td></td>
                  <td><p>Optional. The client&#39;s locale. Complies with the ISO 639-1 standard and defaults to en. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.Vehicle">Vehicle</h3>
        <p>Vehicle details</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>license_plate_number</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The vehicle’s license plate number </p></td>
                </tr>
              
                <tr>
                  <td>vehicle_type</td>
                  <td><a href="#demand.v2.common.Vehicle.VehicleType">Vehicle.VehicleType</a></td>
                  <td></td>
                  <td><p>The vehicle type (standard, limo, van) </p></td>
                </tr>
              
                <tr>
                  <td>make</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The vehicle make </p></td>
                </tr>
              
                <tr>
                  <td>model</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The vehicle model </p></td>
                </tr>
              
                <tr>
                  <td>color</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The vehicle color </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      

      
        <h3 id="demand.v2.common.CancellationInfo.Party">CancellationInfo.Party</h3>
        <p></p>
        <table class="enum-table">
          <thead>
            <tr><td>Name</td><td>Number</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>UNKNOWN</td>
                <td>0</td>
                <td><p>The canceling party is unknown</p></td>
              </tr>
            
              <tr>
                <td>DEMANDER</td>
                <td>1</td>
                <td><p>The client canceled the ride</p></td>
              </tr>
            
              <tr>
                <td>SUPPLIER</td>
                <td>2</td>
                <td><p>The supplier canceled the ride</p></td>
              </tr>
            
          </tbody>
        </table>
      
        <h3 id="demand.v2.common.CancellationInfo.Status">CancellationInfo.Status</h3>
        <p></p>
        <table class="enum-table">
          <thead>
            <tr><td>Name</td><td>Number</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>UNKNOWN_STATUS</td>
                <td>0</td>
                <td><p>The cancellation status is unknown</p></td>
              </tr>
            
              <tr>
                <td>PROCESSING</td>
                <td>1</td>
                <td><p>The cancellation request is being processed</p></td>
              </tr>
            
              <tr>
                <td>ACCEPTED</td>
                <td>2</td>
                <td><p>The cancellation request is accepted</p></td>
              </tr>
            
              <tr>
                <td>REJECTED</td>
                <td>3</td>
                <td><p>The cancellation request is rejected</p></td>
              </tr>
            
          </tbody>
        </table>
      
        <h3 id="demand.v2.common.PublicTransportRouteLeg.PublicTransportMode">PublicTransportRouteLeg.PublicTransportMode</h3>
        <p></p>
        <table class="enum-table">
          <thead>
            <tr><td>Name</td><td>Number</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>UNKNOWN_PUBLIC_TRANSPORT_MODE</td>
                <td>0</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>HIGH_SPEED_TRAIN</td>
                <td>1</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>INTERCITY_TRAIN</td>
                <td>2</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>INTER_REGIONAL_TRAIN</td>
                <td>3</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>REGIONAL_TRAIN</td>
                <td>4</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>CITY_TRAIN</td>
                <td>5</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>BUS</td>
                <td>6</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>FERRY</td>
                <td>7</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>SUBWAY</td>
                <td>8</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>LIGHT_RAIL</td>
                <td>9</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>PRIVATE_BUS</td>
                <td>10</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>INCLINED</td>
                <td>11</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>AERIAL</td>
                <td>12</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>BUS_RAPID</td>
                <td>13</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>MONORAIL</td>
                <td>14</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>WALK</td>
                <td>15</td>
                <td><p></p></td>
              </tr>
            
          </tbody>
        </table>
      
        <h3 id="demand.v2.common.RideOffer.CancellationPolicy">RideOffer.CancellationPolicy</h3>
        <p>Info about the cancellation policy</p>
        <table class="enum-table">
          <thead>
            <tr><td>Name</td><td>Number</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>UNKNOWN_CANCEL_POLICY</td>
                <td>0</td>
                <td><p>Unknown cancellation policy</p></td>
              </tr>
            
              <tr>
                <td>ALLOWED</td>
                <td>1</td>
                <td><p>Cancellation by the client is allowed</p></td>
              </tr>
            
              <tr>
                <td>NOT_ALLOWED</td>
                <td>2</td>
                <td><p>Cancellation by the client is not allowed</p></td>
              </tr>
            
          </tbody>
        </table>
      
        <h3 id="demand.v2.common.RideOffer.SortType">RideOffer.SortType</h3>
        <p>How to sort the returned ride offers</p>
        <table class="enum-table">
          <thead>
            <tr><td>Name</td><td>Number</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>UNKNOWN_SORT_TYPE</td>
                <td>0</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>BY_PRICE</td>
                <td>1</td>
                <td><p>Sort by price (lowest price first)</p></td>
              </tr>
            
              <tr>
                <td>BY_ETA</td>
                <td>2</td>
                <td><p>Sort by arrival time (earliest arrival time first)</p></td>
              </tr>
            
          </tbody>
        </table>
      
        <h3 id="demand.v2.common.RideOffer.TransitType">RideOffer.TransitType</h3>
        <p></p>
        <table class="enum-table">
          <thead>
            <tr><td>Name</td><td>Number</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>UNKNOWN_TRANSIT_TYPE</td>
                <td>0</td>
                <td><p>Unknown transit type</p></td>
              </tr>
            
              <tr>
                <td>TAXI</td>
                <td>1</td>
                <td><p>Taxi offer</p></td>
              </tr>
            
              <tr>
                <td>PUBLIC_TRANSPORT</td>
                <td>2</td>
                <td><p>Public transport offer</p></td>
              </tr>
            
          </tbody>
        </table>
      
        <h3 id="demand.v2.common.RideQuery.RideStatusFilter">RideQuery.RideStatusFilter</h3>
        <p></p>
        <table class="enum-table">
          <thead>
            <tr><td>Name</td><td>Number</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>UNKNOWN_RIDE_STATUS_FILTER</td>
                <td>0</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>PAST</td>
                <td>1</td>
                <td><p>Terminated rides (includes the statuses: COMPLETED, REJECTED or CANCELLED), for the last 72 hours.</p></td>
              </tr>
            
              <tr>
                <td>FUTURE</td>
                <td>2</td>
                <td><p>Pre-booked rides up to 30 minutes before their start time.
(NOTE - the system would automatically update the last_update_time for these rides)</p></td>
              </tr>
            
              <tr>
                <td>ONGOING</td>
                <td>3</td>
                <td><p>Ongoing rides (all rides other than PAST and FUTURE)</p></td>
              </tr>
            
              <tr>
                <td>ALL</td>
                <td>4</td>
                <td><p>All rides</p></td>
              </tr>
            
          </tbody>
        </table>
      
        <h3 id="demand.v2.common.RideQuery.SortType">RideQuery.SortType</h3>
        <p></p>
        <table class="enum-table">
          <thead>
            <tr><td>Name</td><td>Number</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>UNKNOWN_SORT_TYPE</td>
                <td>0</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>UPDATE_TIME_ASC</td>
                <td>1</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>UPDATE_TIME_DESC</td>
                <td>2</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>CREATE_TIME_ASC</td>
                <td>3</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>CREATE_TIME_DESC</td>
                <td>4</td>
                <td><p></p></td>
              </tr>
            
          </tbody>
        </table>
      
        <h3 id="demand.v2.common.RideStatusUpdate.Status">RideStatusUpdate.Status</h3>
        <p>Ride status values</p>
        <table class="enum-table">
          <thead>
            <tr><td>Name</td><td>Number</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>UNKNOWN</td>
                <td>0</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>PROCESSING</td>
                <td>1</td>
                <td><p>Looking for a supplier</p></td>
              </tr>
            
              <tr>
                <td>REJECTED</td>
                <td>2</td>
                <td><p>The supplier cannot fulfill the request. Terminal state.</p></td>
              </tr>
            
              <tr>
                <td>ACCEPTED</td>
                <td>3</td>
                <td><p>A supplier accepted the ride, but a driver is not yet assigned. For a pre-booked ride, this state may last a long while.</p></td>
              </tr>
            
              <tr>
                <td>DRIVER_ASSIGNED</td>
                <td>4</td>
                <td><p>Driver and vehicle are assigned to the ride</p></td>
              </tr>
            
              <tr>
                <td>DRIVER_EN_ROUTE</td>
                <td>5</td>
                <td><p>Vehicle on its way to pickup</p></td>
              </tr>
            
              <tr>
                <td>AT_PICKUP</td>
                <td>6</td>
                <td><p>Vehicle at pickup</p></td>
              </tr>
            
              <tr>
                <td>PASSENGER_ON_BOARD</td>
                <td>7</td>
                <td><p>Vehicle on the way, and passenger on board.</p></td>
              </tr>
            
              <tr>
                <td>AT_DROPOFF</td>
                <td>8</td>
                <td><p>Vehicle arrived at drop-off</p></td>
              </tr>
            
              <tr>
                <td>COMPLETED</td>
                <td>9</td>
                <td><p>Ride finished successfully. Terminal state.</p></td>
              </tr>
            
              <tr>
                <td>CANCELLED</td>
                <td>10</td>
                <td><p>Ride canceled by supplier or demander. Terminal state.</p></td>
              </tr>
            
          </tbody>
        </table>
      
        <h3 id="demand.v2.common.Vehicle.VehicleType">Vehicle.VehicleType</h3>
        <p></p>
        <table class="enum-table">
          <thead>
            <tr><td>Name</td><td>Number</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>UNKNOWN</td>
                <td>0</td>
                <td><p></p></td>
              </tr>
            
              <tr>
                <td>STANDARD</td>
                <td>1</td>
                <td><p>Standard vehicle</p></td>
              </tr>
            
              <tr>
                <td>LIMO</td>
                <td>2</td>
                <td><p>Limousine</p></td>
              </tr>
            
              <tr>
                <td>VAN</td>
                <td>3</td>
                <td><p>Van</p></td>
              </tr>
            
              <tr>
                <td>OTHER</td>
                <td>4</td>
                <td><p>Other vehicle</p></td>
              </tr>
            
              <tr>
                <td>NOT_SUPPLIED</td>
                <td>5</td>
                <td><p>Vehicle type not supplied</p></td>
              </tr>
            
          </tbody>
        </table>
      

      

      
    
      
      <div class="file-heading">
        <h2 id="marketplace/public/grpc/demand_handler/v2/gen-doc/demand_common_types.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_common_types.proto</h2><a href="#title">Top</a>
      </div>
      <p>Basic types.</p>

      
        <h3 id="demand.v2.common.Address">Address</h3>
        <p></p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>country</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>localized country name </p></td>
                </tr>
              
                <tr>
                  <td>country_code</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>ISO 3166-alpha-3 country code </p></td>
                </tr>
              
                <tr>
                  <td>state</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>first subdivision level below the country </p></td>
                </tr>
              
                <tr>
                  <td>county</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>second subdivision level below the country </p></td>
                </tr>
              
                <tr>
                  <td>city</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>primary locality of the address </p></td>
                </tr>
              
                <tr>
                  <td>district</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>subdivision level below the city </p></td>
                </tr>
              
                <tr>
                  <td>sub_district</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>subdivision level below the district; e.g. commonly used in IND </p></td>
                </tr>
              
                <tr>
                  <td>street</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>street name </p></td>
                </tr>
              
                <tr>
                  <td>house_number</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>house number; depending on regional characteristics, can also be house name </p></td>
                </tr>
              
                <tr>
                  <td>postal_code</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>postal code </p></td>
                </tr>
              
                <tr>
                  <td>building</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>building name; e.g. commonly used in HKG </p></td>
                </tr>
              
                <tr>
                  <td>line</td>
                  <td><a href="#string">string</a></td>
                  <td>repeated</td>
                  <td><p>formatted address lines </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.Empty">Empty</h3>
        <p></p>

        

        
      
        <h3 id="demand.v2.common.Location">Location</h3>
        <p>A start/end/midpoint location in a ride</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>point</td>
                  <td><a href="#demand.v2.common.Point">Point</a></td>
                  <td></td>
                  <td><p>Geo-location (latitude and longitude) </p></td>
                </tr>
              
                <tr>
                  <td>address</td>
                  <td><a href="#demand.v2.common.Address">Address</a></td>
                  <td></td>
                  <td><p>Street address. </p></td>
                </tr>
              
                <tr>
                  <td>free_text</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Name of the location if the location is a POI, or an address in a free text format </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.Point">Point</h3>
        <p>A point in the world. Latitude values range from -180 to 180.</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>lat</td>
                  <td><a href="#double">double</a></td>
                  <td></td>
                  <td><p>Latitude </p></td>
                </tr>
              
                <tr>
                  <td>lng</td>
                  <td><a href="#double">double</a></td>
                  <td></td>
                  <td><p>Longitude </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.Price">Price</h3>
        <p>A price value</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>amount</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The price’s numeric amount in decimal format. For example &#34;12.5&#34;, &#34;12&#34;, etc. Unsigned. </p></td>
                </tr>
              
                <tr>
                  <td>currency_code</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The price currency. An ISO 4217 Currency Code, for example: &#34;USD&#34;, &#34;EUR&#34;, &#34;JPY&#34;. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.PriceEstimate">PriceEstimate</h3>
        <p>A price estimate for a ride. Contains only one field value: either a fixed price, or a price range.</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>fixed</td>
                  <td><a href="#demand.v2.common.Price">Price</a></td>
                  <td></td>
                  <td><p>A single fixed price amount </p></td>
                </tr>
              
                <tr>
                  <td>range</td>
                  <td><a href="#demand.v2.common.PriceRange">PriceRange</a></td>
                  <td></td>
                  <td><p>Lower and upper limits of a price range </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.PriceRange">PriceRange</h3>
        <p>A price range. For example, $10.75-$12 will be represented as: { from_amount: "10.75", to_amount: "12", currency_code: "USD"}</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>lower_bound</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The range’s lower limit, for example: &#34;12.5&#34;, &#34;12&#34;, etc. Unsigned. </p></td>
                </tr>
              
                <tr>
                  <td>upper_bound</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The range’s upper limit, for example: &#34;12.5&#34;, &#34;12&#34;, etc. Unsigned. </p></td>
                </tr>
              
                <tr>
                  <td>currency_code</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>The price currency. An ISO 4217 Currency Code, for example: &#34;USD&#34;, &#34;EUR&#34;, &#34;JPY&#34; </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.common.TimeRange">TimeRange</h3>
        <p>A time range</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>from_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>The time range’s lower limit (in milliseconds from epoch time) </p></td>
                </tr>
              
                <tr>
                  <td>to_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>The time range’s upper limit (in milliseconds from epoch time) </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      

      

      

      
    
      
      <div class="file-heading">
        <h2 id="marketplace/public/grpc/demand_handler/v2/gen-doc/demand_s2s_messages.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_s2s_messages.proto</h2><a href="#title">Top</a>
      </div>
      <p></p>

      
        <h3 id="demand.v2.s2s.CancelRideRequest">CancelRideRequest</h3>
        <p>A request to cancel a ride</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>ride_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. The unique ride ID </p></td>
                </tr>
              
                <tr>
                  <td>user_id</td>
                  <td><a href="#google.protobuf.StringValue">google.protobuf.StringValue</a></td>
                  <td></td>
                  <td><p>Optional. The ID of the requesting user </p></td>
                </tr>
              
                <tr>
                  <td>cancel_reason</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Optional. Free text. The reason for the cancellation. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.s2s.CreatePublicTransportRideRequest">CreatePublicTransportRideRequest</h3>
        <p></p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>user_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. The ID of the user. </p></td>
                </tr>
              
                <tr>
                  <td>offer</td>
                  <td><a href="#demand.v2.common.RideOffer">demand.v2.common.RideOffer</a></td>
                  <td></td>
                  <td><p>Mandatory. The chosen public transportation offer. </p></td>
                </tr>
              
                <tr>
                  <td>passenger</td>
                  <td><a href="#demand.v2.common.PassengerDetails">demand.v2.common.PassengerDetails</a></td>
                  <td></td>
                  <td><p>Mandatory. The passenger details at the time of booking </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.s2s.CreateRideRequest">CreateRideRequest</h3>
        <p>A request to create a new ride by offer ID</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>user_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. The user ID for which the ride is created </p></td>
                </tr>
              
                <tr>
                  <td>offer_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. An offer ID that was returned by GetRideOffers() </p></td>
                </tr>
              
                <tr>
                  <td>passenger</td>
                  <td><a href="#demand.v2.common.PassengerDetails">demand.v2.common.PassengerDetails</a></td>
                  <td></td>
                  <td><p>Mandatory. The passenger details at the time of booking </p></td>
                </tr>
              
                <tr>
                  <td>subscribe_to_messages</td>
                  <td><a href="#google.protobuf.BoolValue">google.protobuf.BoolValue</a></td>
                  <td></td>
                  <td><p>Optional. Specifies if messages about the ride will be sent to the passenger. Default is true. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.s2s.GetRecentRidesRequest">GetRecentRidesRequest</h3>
        <p>A request for getting recently-update rides</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>min_update_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Optional. The minimum update time. If this value is supplied, only rides updated AFTER this time are returned.
Otherwise, the default is used (the current time minus 2 hours). </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.s2s.GetRideListByUserRequest">GetRideListByUserRequest</h3>
        <p>A request for getting rises for a specific user</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>query</td>
                  <td><a href="#demand.v2.common.RideQuery">demand.v2.common.RideQuery</a></td>
                  <td></td>
                  <td><p>Optional. Additional query parameters </p></td>
                </tr>
              
                <tr>
                  <td>user_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. The ID of the user whose rides you want to retrieve </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.s2s.GetRideListRequest">GetRideListRequest</h3>
        <p>A request to get a ride list according to query parameters.</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>query</td>
                  <td><a href="#demand.v2.common.RideQuery">demand.v2.common.RideQuery</a></td>
                  <td></td>
                  <td><p>Optional. The query parameters with which to filter the rides returned.
If no query parameters are supplied, the query uses the default values for RideQuery fields (see the RideQuery message documentation). </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.s2s.GetRideLocationRequest">GetRideLocationRequest</h3>
        <p></p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>ride_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. The ride’s unique ID </p></td>
                </tr>
              
                <tr>
                  <td>user_id</td>
                  <td><a href="#google.protobuf.StringValue">google.protobuf.StringValue</a></td>
                  <td></td>
                  <td><p>Optional. The ID of the requesting user </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.s2s.GetRideRequest">GetRideRequest</h3>
        <p>A request to get a ride</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>ride_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. The ride’s unique ID </p></td>
                </tr>
              
                <tr>
                  <td>user_id</td>
                  <td><a href="#google.protobuf.StringValue">google.protobuf.StringValue</a></td>
                  <td></td>
                  <td><p>Optional. The ID of the requesting user </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      
        <h3 id="demand.v2.s2s.RideOffersRequest">RideOffersRequest</h3>
        <p>A request to get ride offers for a given route. If a prebook_pickup_time value is provided, this is a request for a future pickup.</p><p>Otherwise, this is a request for an immediate pickup (within 30 minutes).</p>

        
          <table class="field-table">
            <thead>
              <tr><td>Field</td><td>Type</td><td>Label</td><td>Description</td></tr>
            </thead>
            <tbody>
              
                <tr>
                  <td>user_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Mandatory. The user who is requesting the ride </p></td>
                </tr>
              
                <tr>
                  <td>route</td>
                  <td><a href="#demand.v2.common.Route">demand.v2.common.Route</a></td>
                  <td></td>
                  <td><p>Mandatory. The requested route of the ride. </p></td>
                </tr>
              
                <tr>
                  <td>constraints</td>
                  <td><a href="#demand.v2.common.BookingConstraints">demand.v2.common.BookingConstraints</a></td>
                  <td></td>
                  <td><p>Optional. Ride constraints such as passenger count, child seats, number of suitcases, etc. </p></td>
                </tr>
              
                <tr>
                  <td>prebook_pickup_time_ms</td>
                  <td><a href="#uint64">uint64</a></td>
                  <td></td>
                  <td><p>Optional. An optional future pickup time, which is at least 30 minutes after the request time.
An empty value indicates a request for an immediate ride. </p></td>
                </tr>
              
                <tr>
                  <td>price_range</td>
                  <td><a href="#demand.v2.common.PriceRange">demand.v2.common.PriceRange</a></td>
                  <td></td>
                  <td><p>Optional, unsupported. An optional requested price range. If this value is set, only offers
whose price is within the range are returned. Otherwise, any price is assumed to be acceptable. </p></td>
                </tr>
              
                <tr>
                  <td>sort_type</td>
                  <td><a href="#demand.v2.common.RideOffer.SortType">demand.v2.common.RideOffer.SortType</a></td>
                  <td></td>
                  <td><p>FUTURE FEATURE, CURRENTLY UNSUPPORTED: Optional. How to sort the RideOffers, by price or by ETA.
(The Marketplace default sort order is by best price, and then minimal ETA.) </p></td>
                </tr>
              
                <tr>
                  <td>instance_id</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Optional. The ID of the instance. </p></td>
                </tr>
              
                <tr>
                  <td>passenger_note</td>
                  <td><a href="#string">string</a></td>
                  <td></td>
                  <td><p>Optional. A free text note from the passenger. </p></td>
                </tr>
              
                <tr>
                  <td>transit_options</td>
                  <td><a href="#demand.v2.common.TransitOptions">demand.v2.common.TransitOptions</a></td>
                  <td></td>
                  <td><p>Optional. Parameters for transit offers. </p></td>
                </tr>
              
            </tbody>
          </table>
        

        
      

      

      

      
    
      
      <div class="file-heading">
        <h2 id="marketplace/public/grpc/demand_handler/v2/gen-doc/demand_s2s_service.proto">marketplace/public/grpc/demand_handler/v2/gen-doc/demand_s2s_service.proto</h2><a href="#title">Top</a>
      </div>
      <p>The server 2 service api</p>

      

      

      

      
        <h3 id="demand.v2.s2s.S2SDemandApi">S2SDemandApi</h3>
        <p>A service-to-service API for creating and tracking rides.</p><p>All ride-related entities are created for the current user. The user (or session) is included in the header of all requests.</p><p>=== Normal flow before the ride is created ===</p><p>The client calls GetRideOffers() according to the time, route, price and other constraints that the user specifies.</p><p>The user chooses one ride offer, and the client calls Book().</p><p>The client calls GetRide() repeatedly until the ride status is ACCEPTED.</p><p>=== Normal flow during the ride ===</p><p>The client calls GetRide() repeatedly to get ride status updates.</p><p>The client calls GetRideLocation() repeatedly to get ride location and ETA updates. These calls should be made more frequently, as the location changes continuously.</p><p>=== Flow for getting updates on multiple rides ===</p><p>The client makes an initial call to GetRides() to receive recently updated rides.</p><p>The client repeatedly calls GetRides() to get new updates. Starting from the second call to GetRides(), send the 'to_update_time' from the previous response as the requested minimal update time.</p><p>==== Errors ===</p><p>- NOT_FOUND code – may be returned when an entity doesn’t exist, is expired (such as an offer) or belongs to a different user.</p><p>=== Future Enhancments ===</p><p>Optimization of polling (using ETAG)</p><p>History of rides</p>
        <table class="enum-table">
          <thead>
            <tr><td>Method Name</td><td>Request Type</td><td>Response Type</td><td>Description</td></tr>
          </thead>
          <tbody>
            
              <tr>
                <td>GetRideOffers</td>
                <td><a href="#demand.v2.s2s.RideOffersRequest">RideOffersRequest</a></td>
                <td><a href="#demand.v2.common.RideOffersResponse">.demand.v2.common.RideOffersResponse</a></td>
                <td><p>Get ride offers based on a ride request. May take a few seconds. When no offers are available, returns an empty response.
Errors:
INVALID_ARGUMENT: Invalid field value. For example: prebook_pickup_time is in the past, route.pickup.lat is not a valid latitude, etc.</p></td>
              </tr>
            
              <tr>
                <td>CreateRide</td>
                <td><a href="#demand.v2.s2s.CreateRideRequest">CreateRideRequest</a></td>
                <td><a href="#demand.v2.common.Ride">.demand.v2.common.Ride</a></td>
                <td><p>Create a new ride based on an offer ID. If the offer is valid, a ride is returned immediately with the status PROCESSING.

Errors:
NOT_FOUND: The offer ID is expired or does not exist
ALREADY_EXISTS: A booking already exists for this offer ID (call GetRideOffers to receive new offer IDs).</p></td>
              </tr>
            
              <tr>
                <td>GetRide</td>
                <td><a href="#demand.v2.s2s.GetRideRequest">GetRideRequest</a></td>
                <td><a href="#demand.v2.common.Ride">.demand.v2.common.Ride</a></td>
                <td><p>Get a ride by ID. Use this call to poll for the ride status (every 10 seconds).
NOTE: The status of closed rides (COMPLETED, CANCELLED, REJECTED) never changes.
Errors:
NOT_FOUND: Ride does not exist</p></td>
              </tr>
            
              <tr>
                <td>GetRidesByUser</td>
                <td><a href="#demand.v2.s2s.GetRideListByUserRequest">GetRideListByUserRequest</a></td>
                <td><a href="#demand.v2.common.RideQueryResponse">.demand.v2.common.RideQueryResponse</a></td>
                <td><p>Get rides for a single user.
Returns rides that were updated recently (in the last 3 hours, or after the given from_update_time).</p></td>
              </tr>
            
              <tr>
                <td>GetRides</td>
                <td><a href="#demand.v2.s2s.GetRideListRequest">GetRideListRequest</a></td>
                <td><a href="#demand.v2.common.RideQueryResponse">.demand.v2.common.RideQueryResponse</a></td>
                <td><p>Get rides for all users.
Returns rides that were updated recently (in the last 3 hours, or after the given from_update_time).</p></td>
              </tr>
            
              <tr>
                <td>CancelRide</td>
                <td><a href="#demand.v2.s2s.CancelRideRequest">CancelRideRequest</a></td>
                <td><a href="#demand.v2.common.Empty">.demand.v2.common.Empty</a></td>
                <td><p>Cancel a ride. Returns immediately without waiting for a response from the supplier.
Errors:
NOT_FOUND: Ride does not exist
FAILED_PRECONDITION: Cancel is not allowed by policy, or because the status is REJECTED, COMPLETED, or CANCELLED.</p></td>
              </tr>
            
              <tr>
                <td>GetRideLocationAndEta</td>
                <td><a href="#demand.v2.s2s.GetRideLocationRequest">GetRideLocationRequest</a></td>
                <td><a href="#demand.v2.common.RideLocation">.demand.v2.common.RideLocation</a></td>
                <td><p>Returns the geo-location of the ride. Use this call to poll for the ride location (every 10 seconds)
NOTES:
Test the flag Ride.status_log.is_ride_location_available, to learn whether ride locations are supported.
Rides which are closed (COMPLETED, CANCELLED, REJECTED) never change their location.
Errors:
NOT_FOUND: Ride does not exist</p></td>
              </tr>
            
              <tr>
                <td>CreatePublicTransportRide</td>
                <td><a href="#demand.v2.s2s.CreatePublicTransportRideRequest">CreatePublicTransportRideRequest</a></td>
                <td><a href="#demand.v2.common.Empty">.demand.v2.common.Empty</a></td>
                <td><p>Notify the marketplace that a public transportation offer was chosen</p></td>
              </tr>
            
          </tbody>
        </table>
      
    

    <h2 id="scalar-value-types">Scalar Value Types</h2>
    <table class="scalar-value-types-table">
      <thead>
        <tr><td>.proto Type</td><td>Notes</td><td>C++ Type</td><td>Java Type</td><td>Python Type</td></tr>
      </thead>
      <tbody>
        
          <tr id="double">
            <td>double</td>
            <td></td>
            <td>double</td>
            <td>double</td>
            <td>float</td>
          </tr>
        
          <tr id="float">
            <td>float</td>
            <td></td>
            <td>float</td>
            <td>float</td>
            <td>float</td>
          </tr>
        
          <tr id="int32">
            <td>int32</td>
            <td>Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint32 instead.</td>
            <td>int32</td>
            <td>int</td>
            <td>int</td>
          </tr>
        
          <tr id="int64">
            <td>int64</td>
            <td>Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint64 instead.</td>
            <td>int64</td>
            <td>long</td>
            <td>int/long</td>
          </tr>
        
          <tr id="uint32">
            <td>uint32</td>
            <td>Uses variable-length encoding.</td>
            <td>uint32</td>
            <td>int</td>
            <td>int/long</td>
          </tr>
        
          <tr id="uint64">
            <td>uint64</td>
            <td>Uses variable-length encoding.</td>
            <td>uint64</td>
            <td>long</td>
            <td>int/long</td>
          </tr>
        
          <tr id="sint32">
            <td>sint32</td>
            <td>Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int32s.</td>
            <td>int32</td>
            <td>int</td>
            <td>int</td>
          </tr>
        
          <tr id="sint64">
            <td>sint64</td>
            <td>Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int64s.</td>
            <td>int64</td>
            <td>long</td>
            <td>int/long</td>
          </tr>
        
          <tr id="fixed32">
            <td>fixed32</td>
            <td>Always four bytes. More efficient than uint32 if values are often greater than 2^28.</td>
            <td>uint32</td>
            <td>int</td>
            <td>int</td>
          </tr>
        
          <tr id="fixed64">
            <td>fixed64</td>
            <td>Always eight bytes. More efficient than uint64 if values are often greater than 2^56.</td>
            <td>uint64</td>
            <td>long</td>
            <td>int/long</td>
          </tr>
        
          <tr id="sfixed32">
            <td>sfixed32</td>
            <td>Always four bytes.</td>
            <td>int32</td>
            <td>int</td>
            <td>int</td>
          </tr>
        
          <tr id="sfixed64">
            <td>sfixed64</td>
            <td>Always eight bytes.</td>
            <td>int64</td>
            <td>long</td>
            <td>int/long</td>
          </tr>
        
          <tr id="bool">
            <td>bool</td>
            <td></td>
            <td>bool</td>
            <td>boolean</td>
            <td>boolean</td>
          </tr>
        
          <tr id="string">
            <td>string</td>
            <td>A string must always contain UTF-8 encoded or 7-bit ASCII text.</td>
            <td>string</td>
            <td>String</td>
            <td>str/unicode</td>
          </tr>
        
          <tr id="bytes">
            <td>bytes</td>
            <td>May contain any arbitrary sequence of bytes.</td>
            <td>string</td>
            <td>ByteString</td>
            <td>str</td>
          </tr>
        
      </tbody>
    </table>
  </body>
</html>

